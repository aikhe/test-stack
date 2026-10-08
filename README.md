# test-stack

Vite + React + Tailwind + Convex starter on Bun.

## Stack

- Bun (runtime + package manager)
- React 19 + TypeScript + Vite 8
- Tailwind CSS v4
- Convex backend (local-first dev via `bunx convex dev`)

Planned, not added yet: Zustand (state), TanStack Query (data fetching),
ArkType (validation), auth (Clerk or better-auth).

## Structure

- `convex/` — backend functions (`schema.ts`, `tasks.ts`)
- `src/` — `main.tsx` (Convex provider), `App.tsx`, `index.css` (Tailwind)
- `public/` — static assets

## Dev

- `bun install`
- `bunx convex dev` (terminal 1, keeps backend in sync)
- `bun run dev` (terminal 2)
