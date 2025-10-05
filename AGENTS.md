# Agent Guidelines for haorenjia-site

## Scope
These conventions apply to the entire repository unless a more specific `AGENTS.md` is added in a subdirectory.

## HTML & CSS
- Favor semantic HTML5 structure (`<header>`, `<main>`, `<section>`, `<article>`, `<footer>`), and include accessible affordances such as skip links when you touch layout files.
- Reuse the shared design tokens defined in `hrj/assets/subpage.css` or the inline variables in `index.html` for colors, spacing, and typography. Introduce new tokens only when necessary for consistency.
- External links to the restaurant's navigation should use the Gaode map permalink `https://www.amap.com/place/B023E0YK46` unless a different store is explicitly specified.
- Keep JSON-LD structured data valid JSON (no trailing commas) and update `hasMap` / `sameAs` entries when editing location information.

## Assets & File Organization
- Place reusable front-end assets under `hrj/assets/` and reference them with relative paths from subpages.
- Optimize for fast static hosting: avoid heavy dependencies and prefer pure HTML/CSS/JS solutions.

## Testing & Verification
- After structural or style changes, open the affected HTML in a browser or validator when possible to confirm layout and schema integrity.
- For link updates, double-check that the href resolves to the intended destination.
