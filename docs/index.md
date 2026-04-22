# Documentation Index

This folder holds durable repository guidance for `lightnote-template`.
It should describe the project as it exists today, not placeholder plans.

## Relationship To `AGENTS.md`

- `AGENTS.md` is the working contract for this repository.
- `docs/` stores project-specific guidance that should remain useful across tasks.
- If a topic is not documented here yet, say that it is undocumented instead of inventing a rule.

## Repository Snapshot

- This is an Astro-based static site template for a blog-oriented project.
- `@astrojs/react` and `@astrojs/mdx` are enabled in `astro.config.mjs`.
- Tailwind CSS 4 is wired through the Vite plugin in `astro.config.mjs`.
- Shared theme tokens and global styles live in `src/styles/global.css`.
- shadcn-style UI primitives are configured through `components.json`.
- The current UI surface is still minimal: a single Astro page and a small `ui/` component set.

## Current Source Structure

The main source folders in the repository today are:

- `src/pages/`: route-level Astro pages. Currently includes `index.astro`.
- `src/components/ui/`: reusable UI primitives. Currently includes `button.tsx` and `card.tsx`.
- `src/lib/`: shared utilities such as `utils.ts`.
- `src/styles/`: global styling and theme tokens.
- `public/`: static assets such as favicons.

## Current Commands

Treat `package.json` as the source of truth for runnable commands.

- `bun run dev`: start the local Astro development server
- `bun run build`: build the site for production
- `bun run preview`: preview the production build locally
- `bun run astro`: run Astro CLI commands

## Current Docs

- `docs/index.md`: this index and current repository snapshot
- `docs/commit-convention.md`: Conventional Commits guidance for this repository

## Documentation Gaps

The following areas are not documented in `docs/` yet:

- content authoring workflow for posts, notes, or MDX content
- architecture and source-structure guidance beyond the current high-level snapshot
- page-level design conventions beyond the current starter state
- component usage guidance for the existing `src/components/ui/` primitives

If these areas become stable, add focused documents instead of expanding this file into a catch-all guide.

## Documentation Principles

- Keep docs aligned with the current repository state.
- Prefer small entry points that link to focused detail.
- Document stable constraints and conventions, not one-off task notes.
- Update the relevant doc when a durable workflow or convention changes.
