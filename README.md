# SyntaxWear

Landing page for an e-commerce sneaker brand, developed as the first project in the DobroPass course.

## Overview

This repository contains a static e-commerce landing page for sneakers and athletic footwear, focused on a modern visual style, hero section, product categories, promotional grid, and a footer with newsletter signup and social media links.

The project structure is intentionally simple and based on plain HTML + CSS, without a framework, build system, or backend.

## Technologies

- HTML5
- CSS3
- Static assets in `images/` and `fonts/`
- No Node.js, npm, or bundler dependencies

## Project structure

```text
.
├── css/
│   ├── base.css
│   ├── layout.css
│   ├── variables.css
│   └── components/
│       ├── header.css
│       ├── hero.css
│       ├── product-category.css
│       ├── product-grid.css
│       └── footer.css
├── images/
│   ├── banners/
│   ├── icons/
│   ├── logo/
│   └── products/
├── fonts/
├── index.html
├── README.md
└── .github/
    └── copilot-instructions.md
```

## Main page

The home page is defined in `index.html` and includes:

- fixed header with navigation and icons
- hero banner with main highlight
- category cards for products
- promotional product grid
- footer with newsletter form, links, and social media icons

## Styling and organization

The visual layer is separated by responsibility:

- `css/variables.css` defines visual tokens and fonts
- `css/base.css` contains global rules, buttons, and base layout styling
- `css/components/*.css` organizes visual blocks by interface section
- `index.html` serves as the structural reference for the brand and layout

## Notes

This is a study and interface design project. Most visual and behavioral updates are made directly in HTML and CSS, preserving the static nature of the site.
