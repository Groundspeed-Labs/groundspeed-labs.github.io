## Codex Adapter

This file is the Codex-specific entrypoint for this project.

## Project Summary

- Static Astro site for Groundspeed Labs.
- Hosts the company landing page at `/`.
- Hosts app-specific pages under `src/pages/<app>/`.
- Current live app section: `keepvalid/`.
- Prioritize simplicity, static output, and low-maintenance structure.

## Read This First

When starting work, use this reading order:

1. `README.md`
2. `src/pages/index.astro`
3. `src/pages/keepvalid/index.astro`
4. `src/layouts/BaseLayout.astro`
5. `src/styles/global.css`

Open `openspec/AGENTS.md` when the request involves proposals, planning, larger feature work, or architectural changes.

## Working Rules

- Default to diff-first behavior unless the user explicitly asks you to apply changes.
- Prefer small, targeted edits over broad refactors.
- Keep the site static. Avoid adding runtime JavaScript unless the user explicitly asks for it.
- Do not introduce external runtime dependencies, third-party scripts, analytics, cookies, or hosted fonts.
- Preserve clean URLs and file-based routing under `src/pages/`.
- Keep content direct and no-nonsense. Avoid marketing-heavy copy.

## Project Structure

- `src/pages/index.astro` - company landing page
- `src/pages/keepvalid/index.astro` - KeepValid landing page
- `src/pages/keepvalid/privacy.md` - KeepValid privacy policy
- `src/pages/keepvalid/delete-account.md` - KeepValid account deletion page
- `src/layouts/` - shared page layouts
- `src/styles/global.css` - shared styling
- `public/` - static assets

## Commands

Run commands from the repo root:

- `npm run dev` - start local dev server
- `npm run build` - build the static site
- `npm run preview` - preview the built site

## Validation

Before considering work complete, prefer:

- build verification with `npm run build`
- checking changed pages on both desktop and mobile widths
- verifying internal links still work
- confirming changes do not add external requests or client-side JS unless explicitly intended

## Codex Notes

- Keep Codex-specific behavior in this file.
- Put shared project context in `README.md` or OpenSpec files.
- If this file and `CLAUDE.md` overlap, this file should be treated as the Codex-specific source of truth.

<!-- OPENSPEC:START -->
# OpenSpec Instructions

These instructions are for AI assistants working in this project.

Always open `@/openspec/AGENTS.md` when the request:
- Mentions planning or proposals (words like proposal, spec, change, plan)
- Introduces new capabilities, breaking changes, architecture shifts, or big performance/security work
- Sounds ambiguous and you need the authoritative spec before coding

Use `@/openspec/AGENTS.md` to learn:
- How to create and apply change proposals
- Spec format and conventions
- Project structure and guidelines

Keep this managed block so 'openspec update' can refresh the instructions.

<!-- OPENSPEC:END -->
