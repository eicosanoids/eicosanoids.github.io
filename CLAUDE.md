# Eicosanoids website

This repository is public and builds https://eicosanoids.github.io, the Eicosanoid Atlas: maps of eicosanoids and
related lipid mediators, their production, receptors and regulation (its own site since 2026-11-01, before that the
hidden page /eicosanoid-atlas/ of the Metabolism Regulation website). It holds only finished maps and page text, never
notes, sources or unpublished collaborators' material, and it names no private repository (files, pages, code
comments, commit messages): the maps are built in "a private repository", whose copy script writes them here.

## What comes from where

- Maps, entries, the organisation pages and the click data are copies: `downloads/`, `_maps/`, `pages/`,
  `atlas-data/`, written by the private repository's copy script. Change them there, never here.
- The viewer (`_includes/atlas-app.html`, `atlas-tags.css`), `meta.html`, the page layouts and the styles are copied
  from the Metabolism Regulation website (`VERSION` names the commit). A change to the viewer is made there, where the
  MRegAtlas and the Pattern Atlas use the same code, and copied here.
- The header (name, subtitle, logo) is `_config.yml`, the menu `_data/nav.yml` (an entry with items is a drop-down).
  Every page stays in the menu (user, 2026-11-01). Logo and tab icons come from the favicon skill (the logo is the
  large one, the tab icon `images/favicon/`).

## Addresses (user, 2026-11-01)

`/` the atlas · `/enzyme/`, `/enzyme/layers/`, `/enzyme/list/` · `/branch/`, `/branch/layers/`, `/branch/list/`.

## Rules

- Push to `main`; the site is how the user sees the work.
- The site is kept out of search engines for now (noindex on every page, `_config.yml` defaults).
- Page text as on the Metabolism Regulation map pages: the biology for a reader, no semicolons, no curation notes. The
  Metabolism Regulation Atlas is named MRegAtlas, and links to it are absolute.
- A push that does not show: look at "pages build and deployment" in Actions; when the deploy step fails with "due to
  in progress deployment", re-run the failed jobs of the newest run.
