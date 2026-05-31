# boredpotatoapps.github.io

Public host for **Bored Potato Apps** legal & support pages (privacy policies,
terms, support) referenced by app-store listings.

This is the **only public repo** in the org. App source lives in **private**
repos (`boredpotatoapps/foxriver`, `boredpotatoapps/quackcontrol`, …). Nothing
here exposes app code — just the store-required public pages.

## How it's served

This repo is named `boredpotatoapps.github.io`, so it's the org's GitHub Pages
site. Source: **`main` branch, `/docs` folder** (Settings → Pages).
`/docs` becomes the site root.

```
docs/
  index.html                  -> https://boredpotatoapps.github.io/
  foxriver/
    privacy.html              -> https://boredpotatoapps.github.io/foxriver/privacy.html
  quackcontrol/
    privacy.html              -> https://boredpotatoapps.github.io/quackcontrol/privacy.html
```

## Adding a new app

1. `mkdir docs/<appname>`
2. Add `docs/<appname>/privacy.html` (copy an existing one, edit the app name/details).
3. Optionally `terms.html` / `support.html` in the same folder.
4. Add a link in `docs/index.html`.
5. Commit + push. Use `https://boredpotatoapps.github.io/<appname>/privacy.html`
   in that app's Play / App Store listing.

## Apps

| App | Pages | Source repo (private) |
|-----|-------|-----------------------|
| Fox River | [privacy](https://boredpotatoapps.github.io/foxriver/privacy.html) | `boredpotatoapps/foxriver` |
