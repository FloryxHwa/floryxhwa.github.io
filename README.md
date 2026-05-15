# floryxhwa.github.io

Root site for the Floryx GitHub Pages domain — serves:

- `/` &mdash; the Floryx landing page (`index.html`)
- `/app-ads.txt` &mdash; AdMob app-ads.txt verification per IAB spec
- `/floryx-legal/*` &mdash; legal pages (privacy, account deletion) live in the
  separate `floryx-legal` repo, served at the same domain by GitHub Pages

## Why this repo exists

GitHub Pages serves `https://<user>.github.io/` from a repo named exactly
`<user>.github.io`. The `app-ads.txt` file must live at the *root* of the
developer's domain per the IAB spec, so we cannot put it inside the
`floryx-legal` repo (that one serves at `/floryx-legal/`, not root).

## Updating app-ads.txt

Append new publisher lines to `app-ads.txt` &mdash; the format is one
`<exchange>, <publisher-id>, <relationship>, <cert-id>` per line. Each
new game / monetization partner gets its own line.
