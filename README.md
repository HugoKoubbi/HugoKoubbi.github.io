# Hugo Koubbi Website

This repository contains a personal academic website based on the
[al-folio](https://github.com/alshedivat/al-folio) Jekyll template.

## Main files to edit

- `_config.yml`: site-wide settings, title, URL, footer, and theme options
- `_pages/about.md`: homepage biography
- `_pages/publications.md`: publications page settings
- `_bibliography/papers.bib`: publication entries
- `_data/socials.yml`: email, GitHub, and Google Scholar links

## Local preview

If Ruby and Bundler are installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

If Bundler complains about the locked version, install it first:

```bash
gem install bundler:4.0.4
```

## GitHub Pages deployment

Recommended setup:

1. Create a repository named `HugoKoubbi.github.io`
2. Push this project to the `main` branch
3. In GitHub, go to `Settings` -> `Actions` -> `General` and allow GitHub Actions to run
4. In `Settings` -> `Pages`, set the source to `GitHub Actions`
5. Push to `main` and wait for the `Deploy site` workflow to finish

If you use a different repository name, update `url` and `baseurl` in `_config.yml`.

## Notes

- The current content was seeded from public academic profile pages and publication records.
- Replace the profile photo later by adding your image to `assets/img/` and referencing it in `_pages/about.md`.
- You can add a CV PDF later by setting `cv_pdf` in `_data/socials.yml` or by restoring a dedicated CV page.
