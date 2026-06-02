# support

Public host for **Bored Potato Apps** legal & support pages (privacy policies,
terms, support) referenced by app-store listings.

This is the **only public repo** in the org. App source lives in **private**
repos (`boredpotatoapps/foxriver`, `boredpotatoapps/quackcontrol`, …). Nothing
here exposes app code — just the store-required public pages.

## How it's served

GitHub Pages project site. Source: **`main` branch, `/docs` folder**
(Settings → Pages). The repo name `support` becomes the first URL segment.

```
docs/
  index.html                  -> https://boredpotatoapps.github.io/support/
  foxriver/
    privacy.html              -> https://boredpotatoapps.github.io/support/foxriver/privacy.html
  quackcontrol/
    privacy.html              -> https://boredpotatoapps.github.io/support/quackcontrol/privacy.html
```

## Adding a new app

1. `mkdir docs/<appname>`
2. Add `docs/<appname>/privacy.html` (copy an existing one, edit the app name/details).
3. Optionally `terms.html` / `support.html` in the same folder.
4. Add a link in `docs/index.html`.
5. Commit + push. Use `https://boredpotatoapps.github.io/support/<appname>/privacy.html`
   in that app's Play / App Store listing.

## Apps

| App | Pages | Source repo (private) |
|-----|-------|-----------------------|
| Fox River | [privacy](https://boredpotatoapps.github.io/support/foxriver/privacy.html) | `boredpotatoapps/foxriver` |
| Quack Control | [privacy](https://boredpotatoapps.github.io/support/quackcontrol/privacy.html) | `boredpotatoapps/quackcontrol` |
