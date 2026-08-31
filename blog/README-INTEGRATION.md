# How to integrate this into your existing github.io repo

This is just a folder of Markdown files plus a minimal `_config.yml` — no
build step needed on your end. GitHub Pages builds Jekyll sites automatically
on push.

## If your github.io repo is currently empty or simple

1. Copy everything in this folder into the root of your repo (or into a
   subfolder like `/physics-project/` if you want it separate from an
   existing site — see below).
2. If you don't already have a `_config.yml`, keep the one included here.
   If you do, open both and merge the `theme`, `title`, and `description`
   lines into your existing file rather than replacing it.
3. Commit and push. GitHub Pages will rebuild automatically
   (usually live within a minute or two).

## If you want this as a subsection of an existing site

1. Copy the `physics/`, `neuroscience/`, `claims/`, `index.md`, and
   `about.md` into a subfolder, e.g. `/mystery/`.
2. Update the links inside each page if you nest it (the relative links
   used here — like `../physics/`  — assume the folders sit at the same
   level as shown in this zip; nesting one level deeper means adding
   `../` where needed, or switching to absolute links like
   `/mystery/physics/fields.md`).
3. Add a link to `/mystery/` from your existing homepage nav.

## Adding new pages later

Every page is just a Markdown file with a small header (front matter) like:

```
---
title: Page Title
layout: default
---
```

Add new `.md` files to `physics/`, `neuroscience/`, or `claims/`, and
link to them from the relevant `index.md`. No other setup required —
Jekyll picks up new Markdown files automatically.

## Once it's live

We can walk through:
- git commands to commit and push (`git add`, `git commit`, `git push`)
- checking the GitHub Pages build status/logs if something doesn't render
- any styling tweaks (this uses the free "minima" Jekyll theme by default —
  easy to swap for something else later)
