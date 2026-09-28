# Copilot instructions for SyntaxWear

## Project overview

This repository is a static e-commerce landing page for a sneaker brand called SyntaxWear. It is a design-focused storefront built with plain HTML and CSS, without a JavaScript framework or package manager.

Primary files:

- `index.html` — page structure and content
- `css/base.css` — shared styles, utility classes, and base layout rules
- `css/variables.css` — CSS custom properties for colors and type
- `css/layout.css` — page-level layout helpers
- `css/components/*.css` — section-specific styling for header, hero, product cards, category blocks, and footer
- `images/` — banners, icons, product photography, and logo assets

## Build, test, and lint commands

This repo has no `package.json`, no frontend build system, and no automated test suite.

To preview locally:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

There are no lint or single-test commands to run in this repository.

## High-level architecture

The app is a single static storefront landing page. The structure is intentionally simple:

- `index.html` defines the header, hero, category section, marketing grid, and footer.
- The CSS is split by concern and section so design tokens and component styles remain easy to locate.
- The homepage uses background-image-based panels and CSS grid/flexbox for composition and responsiveness.
- The mobile navigation relies on the existing checkbox toggle pattern in the HTML markup.

Because the site is static, most design changes are done directly in CSS selectors and media queries rather than through application logic.

## Key conventions

- Prefer the existing HTML + CSS patterns already in the repo rather than introducing JS or a framework for simple layout work.
- Reuse existing class names like `.btn`, `.btn-outline`, and `.btn-filled` where the design already uses them.
- Keep stylesheet organization consistent with the current structure: shared rules in `css/base.css`, component rules in `css/components/`.
- Maintain the responsive breakpoints already defined, especially the mobile layout using `@media (max-width: 48rem)`.
- Preserve semantic structure and accessible text: headings, landmarks, and `alt` attributes should remain meaningful.
- When updating assets, keep the related HTML and CSS references in sync.

## Documentation context

The repository is intentionally minimal. Most of the project context lives in the markup and CSS itself, and the README should be treated as a high-level overview rather than a full project specification.

When editing this codebase, assume the project is a static storefront and avoid adding runtime complexity unless the user explicitly requests it.
