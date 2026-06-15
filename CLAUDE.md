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

## Astro Best Practices
- Always use `<Picture />` or `<Image />` from `astro:assets` instead of raw `<img>` tags for raster images — these compile to lightweight `.avif`/`.webp` automatically
- Optimizable images go in `src/assets/images/` (NOT `public/`). Only files that must be served as-is (favicons, OG images, robots.txt) belong in `public/`
- Use scoped `<style>` in components. Leverage all Astro-native features before reaching for external tools

## Conventions
- Fonts: Playfair Display (headings), Open Sans (body), Host Grotesk (nav), Urbanist (UI)
- CSS variables defined in `src/styles/global.css`
- Components in `src/components/`, layouts in `src/layouts/`, pages in `src/pages/`
- Optimizable images in `src/assets/images/`, static assets in `public/`

## Shared Memory
Project memory files are tracked in `.claude/memory/`. These are shared context for all collaborators using Claude Code. See `.claude/memory/MEMORY.md` for the index.
