# AGENTS.md

## Project

TypeScript library starter. ESM-only (`"type": "module"`). Package manager: **pnpm** (enforced by `preinstall` hook).

## Commands

```bash
pnpm dev            # tsdown watch
pnpm build          # tsc --noEmit && tsdown (unbundled output to dist/)
pnpm test           # vitest (globals enabled)
pnpm lint           # eslint (antfu config)
pnpm lint:fix       # eslint --fix
pnpm type:check     # tsc --noEmit
pnpm start          # nr src/index.ts (run source directly)
pnpm commit         # git pull → add → czg interactive → push
```

## Verification order

`pnpm lint` → `pnpm type:check` → `pnpm test` (matches pre-commit hook)

## Conventions

- ESLint: `@antfu/eslint-config`. No Prettier.
- Path alias: `~/*` maps to `src/*` (defined in tsconfig).
- Base tsconfig: `@oiij/tsconfig/tsconfig.json`.
- Tests in `test/` directory, file pattern `*.test.ts`.
- Entry: `src/index.ts`. Output: `dist/index.mjs` + `dist/index.d.mts`.
- Commits: conventional commits via `czg`. Use `pnpm commit` for interactive prompt.
- Pre-commit hook (simple-git-hooks): runs `lint-staged` + `type:check` on staged `*.{js,jsx,ts,tsx}` files.

## Structure

- `src/` — library source code
- `test/` — unit tests (vitest)
- `dist/` — build output (gitignored)
