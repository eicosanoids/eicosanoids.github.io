# Eicosanoids website

This repository is public and builds https://eicosanoids.github.io, the Eicosanoid Atlas: maps of eicosanoids and
related lipid mediators, their production, receptors and regulation (its own site since 2026-11-01, before that the
hidden page /eicosanoid-atlas/ of the Metabolism Regulation website). It holds only finished maps and page text, never
notes, sources or unpublished collaborators' material, and it names no private repository (files, pages, code
comments, commit messages): the maps are built in "a private repository", whose copy script writes them here.

## What comes from where

- Maps, entries, the organisation pages and the click data (`downloads/`, `_maps/`, `pages/`, `atlas-data/`) are not in
  this repository (since 2026-11-14): they are kept in a private data repository, written by the private repository's
  copy script, and put into the site by the workflow `.github/workflows/build.yml` when it is built (secret
  `DATA_TOKEN`, read-only). Change them there, never here; after the data changes, run the workflow by hand.
- The viewer (`_includes/atlas-app.html`, `_includes/atlas-tags.css`) is a copy of the viewer's source
  (https://viewer-source.github.io, since 2026-11-09; `_includes/VERSION` names its commit): never edited here, a change
  is made in the source and copied with its `copy-to-site.sh`. `meta.html`, the page layouts and the styles are copied
  from the Metabolism Regulation website (`VERSION` names the commit).
- The header is a top bar (user, 2026-11-10, as the next Metabolism Regulation version): the name (`_config.yml`)
  and the menu (`_data/nav.yml`, an entry with items is a drop-down), a thin line under it, as wide as the viewer; no
  subtitle (`description` stays for the page's meta description).
  Every page stays in the menu (user, 2026-11-01). No logo in the header (user, 2026-11-01: removed; `images/logo.svg`
  kept, shown again by `avatar:` in `_config.yml`). Tab icons come from the favicon skill (`images/favicon/`).

## Addresses (user, 2026-11-01)

`/` the atlas · `/enzyme/`, `/enzyme/layers/`, `/enzyme/list/` · `/branch/`, `/branch/layers/`, `/branch/list/`.

## Rules

- Push to `main`; the site is how the user sees the work.
- The site is kept out of search engines for now (user, 2026-11-01: hidden; noindex on every page, `_config.yml` defaults).
- Page text as on the Metabolism Regulation map pages: the biology for a reader, no semicolons, no curation notes. The
  Metabolism Regulation Atlas is named MRegAtlas, and links to it are absolute.
- A push that does not show: look at "Build with data" in Actions (the Pages source is GitHub Actions; a "pages build
  and deployment" run there means the source was set back to a branch, which deploys the site without its data).
