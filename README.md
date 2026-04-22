# lightnote-template

`lightnote-template` is a lightweight Astro starter for a statically generated, blog-oriented site.

The repository currently includes:

- Astro 6 for routing and static builds
- React integration for interactive UI components
- MDX integration for content authoring
- Tailwind CSS 4 for styling
- shadcn-style UI primitives configured through `components.json`

## Project Structure

The current source tree is intentionally small:

```text
/
├── docs/
│   ├── commit-convention.md
│   └── index.md
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── components/ui/
│   │   ├── button.tsx
│   │   └── card.tsx
│   ├── lib/utils.ts
│   ├── pages/index.astro
│   └── styles/global.css
├── astro.config.mjs
├── components.json
└── package.json
```

## Commands

Use the scripts defined in `package.json`:

| Command | Purpose |
| :------ | :------ |
| `bun run dev` | Start the local Astro development server |
| `bun run build` | Build the site for production |
| `bun run preview` | Preview the production build locally |
| `bun run astro` | Run Astro CLI commands |

## Documentation

- [docs/index.md](./docs/index.md): repository documentation index and current project snapshot
- [docs/commit-convention.md](./docs/commit-convention.md): Conventional Commits guidance for this repository

## Current Status

This template is still close to a starter project. It has a minimal homepage, shared styling setup, and a small set of UI primitives. Content collections, blog authoring workflow, and broader architecture conventions are not documented yet.
