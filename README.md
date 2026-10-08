# test-stack

Vite + React + Tailwind + Convex starter on Bun.

## Stack

- Bun (runtime + package manager)
- React 19 + TypeScript + Vite 8
- Tailwind CSS v4
- Convex backend (local-first dev via `bunx convex dev`)
- Clerk auth (`VITE_CLERK_PUBLISHABLE_KEY` + a `convex` JWT template)
- Zustand (UI state, `src/store.ts`), TanStack Query (non-Convex data,
  `src/lib/queryClient.ts`), ArkType (validation, `src/lib/validators.ts`)

## Structure

- `convex/` — backend functions (`schema.ts`, `tasks.ts`)
- `src/` — `main.tsx` (Convex provider), `App.tsx`, `index.css` (Tailwind)
- `public/` — static assets

## Dev

- `bun install`
- `bunx convex dev` (terminal 1, keeps backend in sync)
- `bun run dev` (terminal 2)
