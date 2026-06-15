---
name: Always use Astro best practices
description: Use Astro-native features like <Picture />, <Image /> from astro:assets for automatic .avif/.webp optimization
type: feedback
---

Always use Astro best practices. Key examples:
- Use `<Picture />` or `<Image />` from `astro:assets` instead of raw `<img>` tags for raster images. These compile to lightweight .avif/.webp automatically.
- Images that need optimization go in `src/assets/` (not `public/`) so the build pipeline processes them.
- `public/` is only for files that must be served as-is (favicons, robots.txt, etc).

**Why:** User explicitly requires Astro best practices at all times. The image pipeline is a core Astro feature that significantly improves performance.

**How to apply:** Before writing any `<img>` tag, consider whether it should be a `<Picture />` or `<Image />` component. Import images from `src/assets/` in frontmatter. Reserve `public/` for non-optimizable assets.
