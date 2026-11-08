# Patch Notes fruit stills

JPEG portraits the [Patch Notes](https://patch-notes.grok.me) archive shows.
Copied from the private app repo so Publish does not have to upload 200 MB.

Fanatic stills are a personal-copy grant (August 2026). Weigh-off stills are
private-archive keeps. Do not treat this tree as a crawl target.

This snapshot does not relicense those stills, grant crawl or reuse rights, or
replace the personal-copy / private-archive terms above. Do not copy, scrape,
or republish the JPEGs from GitHub, from any CDN of this tree, or from the
live app.

## Source and status

This is a **public companion asset snapshot** for Patch Notes. It is not the
application. The app's canonical source is a separate private repository.
This tree does not publish that source or its configuration.

Canonical GitHub `main` for this snapshot:
`cdbc2ddb45b10ae15120c9bf84b85b0da2b0d660`
(last GitHub push 2026-09-25 01:17 UTC; 2026-09-24 evening in US timezones).

### GitHub snapshot vs live hosting

Public evidence only (checked 2026-11-08). This is not a claim that hosting
has migrated, that GitHub is exhaustive, or that live display matches this
tree.

- This repository is a **GitHub-hosted JPEG snapshot**. GitHub Pages is not
  enabled. The live site origin `https://patch-notes.grok.me` does not itself
  serve these files (HEAD of `/archive-photos/...` on that host returned 404).
- Public app JavaScript on that site (version string `0.19.0`) prefixes
  `/archive-photos/` paths with
  `https://cdn.jsdelivr.net/gh/Brianccmc/patch-notes-photos@main` (jsDelivr
  CDN of this GitHub `main`). That is the only public stills-host prefix found
  in the bundle.
- **Cloudflare R2 is not named** in that public bundle. This label does not
  assert that the live app currently serves stills from R2, or that any
  migration off GitHub/jsDelivr is complete.

### Public-app parity: unverified

Do not treat this collection as exhaustive, or as a 1:1 match to what the
live app displays. A public filename check on 2026-11-08 found live JS
`/archive-photos/` names that exist in this snapshot, but some of those files
sit at the repository root rather than under `archive-photos/`. A sampled
jsDelivr URL using the live `/archive-photos/` prefix returned 404 for a
root-only file. Other files under `archive-photos/` were not referenced in
that public JS. Path layout versus live display is therefore unverified.
