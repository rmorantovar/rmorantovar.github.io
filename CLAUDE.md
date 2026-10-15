# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal academic website (Roberto Morán-Tovar) built with Jekyll and the `minima` theme, served via GitHub Pages from `main`. There is no CI workflow, test suite, or linter; pushing to `main` publishes the site.

## Commands

```sh
bundle install              # install Jekyll 4.4 + minima + jekyll-feed
bundle exec jekyll serve    # local preview at http://localhost:4000 (restart after editing _config.yml)
bundle exec jekyll build    # build into _site/ (gitignored)
```

## Structure

- **Main site**: Markdown pages at the root (`index.markdown`, `about.md`, `research.md`, `biophys_archive.md`) use minima's `default` layout. The top nav is controlled by `header_pages` in `_config.yml` — a new page only appears in the header if added there. `_includes/footer.html` overrides minima's footer (adds Bluesky and Google Scholar links driven by `_config.yml` vars); other includes/layouts come from the gem theme.
- **Biophysics archive**: a Jekyll collection (`_biophys_archive/`, output at `/biophys_archive/:name/`). Each entry is a Markdown file with front matter `title`, `authors`, `year`, `journal`, `paper_link`; `biophys_archive.md` lists them sorted by `year`. Filenames follow `YEAR_AuthorInitialLastname_topic.md`.

## Notes

- `research.md` has permalink `/reseach/` (typo) — changing it alters the public URL.
- `_layouts/polla.html` is a leftover from the removed World Cup prediction pool ("Polla Mundialista"); nothing uses it now. The pool's pages are in git history (last at `d61c60d`) if they need restoring.
