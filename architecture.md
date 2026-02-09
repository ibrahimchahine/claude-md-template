# Architecture

<!-- This file is loaded by Claude on-demand via progressive disclosure.
     It is NOT read every session — only when relevant to the task.
     Keep it focused: 1-2 pages max. Use file:line pointers, not code snippets. -->

## Overview
<!-- What does this system do? One paragraph max. -->

## Tech Stack
<!-- List your core technologies -->
- **Runtime**: <!-- e.g., Node.js 20, Python 3.12 -->
- **Framework**: <!-- e.g., Next.js 14, FastAPI -->
- **Database**: <!-- e.g., PostgreSQL via Prisma, MongoDB -->
- **Key Services**: <!-- e.g., Stripe, OpenAI API, AWS Lambda -->

## Service Map
<!-- How do the main pieces connect? Keep it simple. -->
<!-- Example:
     Client → API Gateway → Auth Service → Database
                          → Payment Service → Stripe
                          → AI Service → OpenAI -->

## Data Flow
<!-- How does data move through the system? -->
<!-- Example:
     1. User uploads document via /api/upload
     2. Lambda processes and chunks the document (see src/services/chunker.ts:15)
     3. Embeddings generated and stored in vector DB
     4. Query hits /api/search → retrieval → LLM response -->

## Key Files
<!-- Point Claude to the most important files it should understand -->
<!-- Example:
     - src/services/auth.ts — Authentication logic (has retry workaround at line 45)
     - src/db/schema.prisma — Database schema (source of truth)
     - src/api/webhooks/stripe.ts — MUST validate signatures before processing -->

## Gotchas
<!-- Project-specific warnings that prevent costly mistakes -->
<!-- Example:
     - The /legacy endpoint uses a different auth flow — see docs/legacy-auth.md
     - Never modify migrations directly — always use `prisma migrate dev`
     - Image uploads go to Cloudinary, not local storage -->
