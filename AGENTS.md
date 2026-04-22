# AGENTS.md

This repository is a template project for a statically generated blog built on Astro.

## 1. Read Before Implementation

Before any non-trivial task:

1. Read `docs/index.md`
2. Read any task-relevant docs in `docs/`
3. Check `package.json` scripts before deciding how to run or verify changes

If the needed documentation does not exist, say so explicitly instead of inventing project rules.
Do not claim to have read documents that do not exist.

## 2. Plan Non-Trivial Tasks

For non-trivial tasks, briefly state:

1. what will change
2. how it will be verified
3. any assumptions or risks

## 3. Project Structure Rules

Follow Astro conventions unless project documents specify otherwise.

### Pages And Routes

- Prefer putting route-level pages in `src/pages/`
- Do not create new routing conventions without a clear reason

### Components

- Put reusable UI pieces in `src/components/` or the existing component location
- Avoid creating many tiny wrapper components with no real reuse value

### Static Assets

- Put static assets in `public/` unless there is an existing different pattern

## 4. Implementation Rules

### Preserve Blog Clarity

This is a blog-oriented repository.
Prefer readable structure over premature abstraction.

### Avoid Framework Drift

- Do not introduce patterns from other frameworks unless clearly needed
- Do not convert the project structure into a different app architecture without being asked

### Keep Changes Aligned With User Intent

Every changed file should map directly to the request.

### No Speculative Features

Do not introduce new large subsystems or infrastructure unless explicitly requested or already documented as part of the project plan.
Examples include CMS integrations, analytics, i18n, complex theme systems, or content-pipeline overhauls.

## 5. Verification

Before finishing:

- Use the scripts that actually exist in `package.json`
- Prefer minimal valid verification for the task
- For build-affecting changes, run `bun build`
- If a script does not exist, do not pretend it passed

If verification could not be completed, state:

- what was not verified
- why
- what risk remains

## 6. Documentation Updates

If your change affects:

- repository structure
- authoring workflow
- component usage patterns
- theme or layout conventions
- commit rules

then update the relevant file in `docs/`.

If the documentation is missing, mention the missing doc and suggest the file that should be added.

## 7. Output Requirements

When finishing a task, explain:

- what changed
- why it changed
- which files were touched
- what was verified
- any assumptions, unverified items, or remaining risks

## 8. Current Known Commands

Use the actual scripts defined in `package.json`:

- `bun dev`
- `bun build`
- `bun preview`
- `bun astro`

Do not assume lint or test scripts exist unless they are added later.
If scripts and docs disagree, follow the scripts that actually exist in `package.json`.
