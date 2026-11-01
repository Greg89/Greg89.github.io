# Greg89.github.io

Developer portfolio and public reference site for my applications, served by GitHub Pages at
**https://greg89.github.io**.

Each app gets stable URLs you can give to Stripe (or app stores, OAuth consent screens, etc.):

| Purpose | URL |
|---|---|
| Business / product website | `https://greg89.github.io/apps/<app-id>/` |
| Privacy policy | `https://greg89.github.io/apps/<app-id>/privacy/` |
| Terms of service | `https://greg89.github.io/apps/<app-id>/terms/` |
| Refund policy | `https://greg89.github.io/apps/<app-id>/refunds/` |
| Customer support | `https://greg89.github.io/contact/` |

## Adding an app

1. Add an entry to `_data/apps.yml` (copy `example-app`).
2. Copy `apps/example-app/` to `apps/<app-id>/` and change `app:` and `title:` in each file.
3. Commit and push — GitHub Pages rebuilds automatically.

Owner details shared by every page (name, support email, jurisdiction) live under `owner:` in `_config.yml`.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

## Enabling GitHub Pages

Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main` / `(root)`.

> The legal pages are generic templates, not legal advice. Review them for your situation.
