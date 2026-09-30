# Personal GitHub Pages Site

This is a Jekyll site prepared for GitHub Pages.

## Site structure

- `index.md`: shared research identity and a short introduction.
- `_layouts/home.html`: brief research areas, profile icons, and compact international publications.
- `_data/research.yml`: Robot Foundation Models, Embodied AI & Robot Learning, Efficient AI Systems.
- `_data/projects.yml`: ongoing robot inference, HeMeR, and FCGraft descriptions.
- `_data/publications.yml`: complete author lists, venues, and verified links.
- `_includes/publications.html`: shared compact/full publication renderer; titles are plain text.
- `research.md`: research narrative and project details.
- `publications.md`: all five publications, grouped and numbered by international/domestic venue.
- `about.md`: research trajectory and a link to the full academic CV.
- `assets/pdf/Saehun_Chun_CV.pdf`: public academic CV, copied from `../CV/sep_update/` after rebuilding.
- `_config.yml`: metadata, external profiles, and navigation.
- `assets/css/main.css`: responsive single-column layout.

Home shows full author lists beneath publication titles and omits selected-project descriptions, domestic papers, GPA, and teaching details. Full
publication records remain under Publications; teaching and older projects remain
in the academic CV. No unverified metrics, skills, profile links, or demo assets
are published. Paper links are separate from non-clickable titles.

## Local setup

```bash
bundle install
bundle exec jekyll serve
```

## Deploy

1. Rename this repository to `YOUR_GITHUB_USERNAME.github.io` for a user site, or keep any repository name and enable GitHub Pages for a project site.
2. Replace the placeholder profile values in `_config.yml`.
3. Push the repository to GitHub.
