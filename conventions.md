# Code Conventions

<!-- This file is loaded by Claude on-demand via progressive disclosure.
     Only include patterns that Claude consistently gets wrong.
     If Claude already follows a convention from your existing code, don't document it here —
     LLMs are in-context learners and will match existing patterns. -->

## Patterns to Follow
<!-- Example:
     - Use named exports, not default exports
     - Error handling: always use try-catch with async/await, never swallow errors
     - State management is handled by Zustand — see src/stores/ for examples
     - New components require a corresponding test file using [your test framework] -->

## Patterns to Avoid
<!-- Always provide the preferred alternative — "never do X" alone causes Claude to get stuck -->
<!-- Example:
     - Don't use `any` type — use explicit types or `unknown` with type guards
     - Don't put business logic in API route handlers — extract to src/services/
     - Don't use relative imports across module boundaries — use path aliases (@/...) -->

## Naming
<!-- Example:
     - Files: kebab-case (user-profile.ts)
     - Components: PascalCase (UserProfile.tsx)
     - Functions/variables: camelCase
     - Database tables: snake_case
     - Environment variables: SCREAMING_SNAKE_CASE -->

## Git
<!-- Example:
     - Branch naming: feature/TICKET-123-short-description
     - Commit messages: Conventional Commits (feat:, fix:, chore:)
     - Never push directly to main — always use feature branches -->
