# Project: <!-- Your Project Name -->

<!-- One-liner: what is this project and what stack does it use? -->
<!-- Example: SaaS dashboard built with Next.js 14, TypeScript, Prisma, and Stripe. -->

## Commands
```
<!-- Replace with your actual commands -->
npm run dev          # Start dev server
npm run build        # Production build
npm run test         # Run tests (prefer single test files over full suite)
npm run lint         # Lint + format
```

## Structure
<!-- Update to match your project layout -->
- `/src` — Application source code
- `/tests` — Test files
- `/docs` — Architecture, conventions, and deep-dive references
- `/tasks` — Plans, todos, and lessons learned

## Context
**IMPORTANT:** Before starting any task, check which docs below are relevant and read them first.
- `docs/architecture.md` — System design, service boundaries, data flow
- `docs/conventions.md` — Code patterns, naming rules, project-specific gotchas
- `tasks/lessons.md` — Known pitfalls and prevention rules from past mistakes

## Workflow

### Planning
- Use plan mode for any task with 3+ steps or architectural decisions
- Write plan to `tasks/todo.md` with checkable items and acceptance criteria before coding
- If implementation goes off-track, STOP — re-plan instead of pushing through

### Verification
- Never mark a task complete without proving it works
- Run tests, check logs, verify the actual behavior
- Clean up: no debug code, temp files, or leftover console.logs in final output

### Learning
- After ANY user correction: add the pattern + prevention rule to `tasks/lessons.md`
- If a mistake repeats, escalate it to the Do Not section of this file

## Principles
- **Simplicity**: Smallest change that solves the problem. Minimal code footprint.
- **Root Causes**: Fix the real issue; never apply band-aid patches.
- **Minimal Blast Radius**: Only touch files relevant to the current task.
- **Autonomy**: Given a bug report, trace the error, find the cause, fix it. Ask the user only when truly blocked — and when you do, ask one question with a recommended default.

## Compaction
When compacting, always preserve: the list of modified files, current `tasks/todo.md` state, any failing tests, and the active plan.

## Do Not
- Skip tests before marking a task done — run them first
- Add hacky/temporary fixes without clearly flagging them — prefer clean solutions
- Modify files outside the current task's scope — ask before expanding scope
- Silently swallow errors — log or propagate them
<!-- Add project-specific rules below as you discover them -->
