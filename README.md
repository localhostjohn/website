# Stash — Jekyll Conversion (Best-Effort)

This folder contains a best-effort conversion of a WordPress theme into a Jekyll site/theme scaffold.

## What was done

- Created a Jekyll structure: `_layouts`, `_includes`, `assets`, `_posts`, and config files.
- Attempted **mechanical** conversion of common WordPress template tags and The Loop to Jekyll Liquid equivalents.
- Copied assets (CSS/JS/images) where found.
- Appended converted snippets from key PHP templates (index.php, single.php, page.php, archive.php, header.php, footer.php) into the Jekyll layouts/includes as comments & HTML.

> ⚠️ This conversion is intentionally conservative. Manual review is recommended, especially for menus, widgets, shortcodes, custom queries, ACF fields, and any plugin-dependent features.

## Quick Start

1. Ensure Ruby is installed.
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Run locally:
   ```bash
   bundle exec jekyll serve
   ```
4. Visit `http://localhost:4000`

## Notes & Next Steps

- Navigation: Replace the placeholder nav in `_includes/header.html`. A nice approach is to create `_data/navigation.yml` and iterate through it.
- Pagination uses `jekyll-paginate-v2`. Make sure it's enabled in `_config.yml` and front matter where needed.
- If your original theme used custom post types, shortcodes, or dynamic widgets, replicate with Jekyll collections/data files or strip them.

## Attribution

Converted from WordPress theme **Stash** by ThemeBeans (https://themebeans.com/themes/stash).