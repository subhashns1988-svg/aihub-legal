# AI Hub — legal pages

Public hosting for the two URLs the Google Play Console requires:

| Page | URL |
|---|---|
| Privacy policy | `https://<owner>.github.io/aihub-legal/privacy-policy.html` |
| Account deletion | `https://<owner>.github.io/aihub-legal/delete-account.html` |

## Why this repo is separate, and public

The AI Hub app repo is **private**. GitHub Pages served from a private repo is not
publicly reachable, so Play's reviewers — and users — would get a 404 or a login
wall where the policy should be. This repo exists purely to make those two pages
anonymously readable, and contains nothing else: no app source, no keys, no
config.

## Keeping it in sync

`privacy-policy.html` is a **copy**. The source of truth is `docs/privacy-policy.md`
in the app repo, with `docs/privacy-policy.html` as its HTML mirror. When the
policy wording changes:

1. Edit `docs/privacy-policy.md` in the app repo.
2. Mirror the change into `docs/privacy-policy.html` there.
3. Copy that file here and push.

Skipping step 3 means the published policy is the stale one, which is the failure
mode worth guarding against — Play links to *this* copy.

`delete-account.html` lives only here. It has to be readable by someone who has
already uninstalled the app, so it spells out the in-app steps rather than linking
into the app.

## Constraints these pages are built to

- **No build step and no external requests.** No CDN fonts, no scripts, no shared
  stylesheet. Each page is self-contained, so nothing on a reviewer's network can
  make it fail to render.
- **Deletion instructions must stand alone.** Someone who has removed the app still
  needs to know how to delete the account, hence the email fallback.
