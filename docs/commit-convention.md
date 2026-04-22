# Commit Convention

This repository uses Conventional Commits for Git commit messages.

## Format

Use this format:

```text
<type>(<scope>): <subject>
```

Example:

```text
fix(auth): prevent duplicate login submit
```

## Types

Use one of the following commit types:

- `feat`: a user-facing feature or capability
- `fix`: a bug fix or behavioral correction
- `refactor`: internal code restructuring without intended behavior change
- `docs`: documentation-only changes
- `test`: adding or updating tests
- `chore`: maintenance work that does not fit the categories above

## Scope

The scope should name the main area affected by the change.

Prefer short scopes such as:

- `auth`
- `editor`
- `notes`
- `ui`
- `docs`
- `build`

Guidelines:

- Use a single scope when one area is clearly primary.
- If multiple areas are touched, choose the most behaviorally significant one.
- Omit the scope only if no clear scope exists and the project prefers that style.

## Subject

The subject line should:

- be written in English
- use imperative mood
- stay concise
- avoid a trailing period

Good examples:

- `feat(editor): add slash command menu`
- `fix(ui): align toolbar actions on mobile`
- `docs(readme): clarify local development steps`

Bad examples:

- `feat(editor): added slash command menu`
- `fix(ui): fixes toolbar alignment issue.`
- `chore: some updates`

## Body

Add a body for non-trivial changes.

The body should explain why the change was needed, especially when the reason is not obvious from the diff or subject line alone.

Example:

```text
fix(editor): preserve cursor after auto-save

Auto-save was reinitializing the editor state, which caused the
selection to jump to the start of the document during longer edits.
```

## Choosing The Type

Use this quick guide:

- visible product behavior changed: `feat` or `fix`
- structure changed without intended behavior change: `refactor`
- only documentation changed: `docs`
- only tests changed: `test`
- tooling, dependency, or maintenance work: `chore`

## Rules For Agents

When an agent is asked to create a commit:

- default to this convention unless the user explicitly requests another format
- choose the narrowest accurate type
- avoid vague subjects
- include a body when the reasoning behind the change is not obvious
