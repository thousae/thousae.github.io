# Personal GitHub Pages Site

This is a Jekyll site prepared for GitHub Pages.

## Site structure

- `index.md`: home-page research overview and current focus.
- `_layouts/home.html`: profile/contact sidebar and selected publications.
- `about.md`, `research.md`: detailed biography and research/publications.
- `_config.yml`: profile details, external links, and navigation.
- `assets/css/main.css`: shared styles, desktop columns, and mobile layout.

The home page uses a compact profile sidebar alongside research information and
selected papers. On mobile, these sections stack in a single column with normal
page scrolling.

## Local setup

```bash
bundle install
bundle exec jekyll serve
```

## Deploy

1. Rename this repository to `YOUR_GITHUB_USERNAME.github.io` for a user site, or keep any repository name and enable GitHub Pages for a project site.
2. Replace the placeholder profile values in `_config.yml`.
3. Push the repository to GitHub.
