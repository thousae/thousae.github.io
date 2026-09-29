# Personal GitHub Pages Site

This is a Jekyll site prepared for GitHub Pages.

## Site structure

- `index.md`: short home-page introduction.
- `_layouts/home.html`: profile links and complete publication list.
- `_data/publications.yml`: shared publication records for Home and Research.
- `_includes/publications.html`: numbered publication groups, author names, and venue details.
- `research.md`: research directions and publication descriptions with stable paper anchors.
- `about.md`: biography, education, experience, teaching, and contact.
- `_config.yml`: profile details, external links, and navigation.
- `assets/css/main.css`: single-column layout and responsive typography.

Home presents the introduction and all papers in a compact reading layout. Paper
titles link to their Research entries; About contains the longer biography and
career details. Publication records are updated once in the shared YAML file.

## Local setup

```bash
bundle install
bundle exec jekyll serve
```

## Deploy

1. Rename this repository to `YOUR_GITHUB_USERNAME.github.io` for a user site, or keep any repository name and enable GitHub Pages for a project site.
2. Replace the placeholder profile values in `_config.yml`.
3. Push the repository to GitHub.
