# Claude Code Project Rules

## Autonomy
- Claude has full autonomy over GitHub operations and all files in this project directory.
- Do NOT touch computer or system-level settings.

## GitHub Workflow
1. **Create a branch** off `main` for any new work.
2. **Work and build** on that branch.
3. **Commit** to the branch (frequently).
4. **Create a PR** when the work is ready for review.
5. **NEVER merge a PR** without explicit approval from a collaborator.

## Tech Stack
- **Astro** with TypeScript (strict)
- **Cloudflare Pages** with `@astrojs/cloudflare` adapter (server mode)
- **Scoped CSS** on Astro components — no CSS frameworks or JS frameworks
- **No CMS** — content is published directly through Claude

## Conventions
- Fonts: Playfair Display (headings), Open Sans (body), Host Grotesk (nav), Urbanist (UI)
- CSS variables defined in `src/styles/global.css`
- Components in `src/components/`, layouts in `src/layouts/`, pages in `src/pages/`
- Images go in `public/images/`
