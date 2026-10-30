# Trouble Quest

Internal trouble-ticketing app for the user's company.

## Stack
- Frontend: React + TypeScript (Vite), in `src/`
- Middleware/API: Express
- Database: PostgreSQL (local install)
- Single repo / single project folder for everything (no separate client/server repos)

## How we work
- Build in small, testable chunks, one per user prompt. Do only what the prompt asks: no extra features, scaffolding, or refactors.
- After each chunk, state how to verify it. The user tests with direct PostgreSQL checks, Postman, and the browser.
- Ask before adding any other kind of check (automated tests, lint rules, scripts, etc.).

## Notes
- TypeScript is pinned to `~6.0.0` because typescript-eslint 8.x requires `<6.1.0`. Don't upgrade to TS 7 until typescript-eslint supports it.
- Commands (`npm run dev`, `build`, `lint`) are in `package.json`. Add server and DB commands here as they are created.
