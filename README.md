# ARTICULATE website

This is the Jekyll website for ARTICULATE: Science in your own language.

## Local preview

Install Ruby and Bundler, then run:

```powershell
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` in a browser.

## GitHub Pages

The `github-pages` gem in the `Gemfile` matches the GitHub Pages build environment. Push the repository to GitHub, then enable **Settings > Pages > Deploy from a branch** and select the branch containing this site.

## Updating the team

Add or edit entries in `_data/researchers.yml`. To include a headshot, place the image in `assets/images/team/`, then set `photo` to the relative path, for example:

```yml
photo: /assets/images/team/yolanda-vazquez-alvarez.jpg
```

Use an image with a square crop and ensure permission has been obtained before publishing.

## Adding publications

Add a PDF under `assets/publications/` and create an entry in `_data/publications.yml`:

```yml
- type: Conference paper
  title: Publication title
  authors: Author One, Author Two, and Author Three
  pdf: /assets/publications/publication.pdf
```