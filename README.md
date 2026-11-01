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

## Included apps

| App | Overview | Source |
|---|---|---|
| HousePoints | [Overview](https://greg89.github.io/apps/housepoints/) | [Repository](https://github.com/Greg89/HousePoints) |
| CurateDS | [Overview](https://greg89.github.io/apps/curateds/) | [Repository](https://github.com/Greg89/CurateDS) |
| Normaize | [Overview](https://greg89.github.io/apps/normaize/) | [Client](https://github.com/Greg89/normaize-client), [API](https://github.com/Greg89/normaize-server) |

All three are listed as **In development**, with no paid plans announced.
Live application URLs are omitted until confirmed. Each overview has privacy,
terms, and refund-policy links. The example app is no longer published.

## Adding an app

1. Add an entry to `_data/apps.yml` using an existing app as a starting point.
2. Copy an existing folder under `apps/` to `apps/<app-id>/` and change `app:` and `title:` in each file. Update overview content for the new app.
3. Commit and push — GitHub Pages rebuilds automatically.

Only add `url:` after confirming the live app address. Omit `payments:` until
paid plans are ready; pages without it display the pre-launch pricing/refund
notice. Before enabling billing, add the confirmed processor, currency, and
`plans` (each with `name`, `price`, and `details`), plus `refunds.window_days` and
`refunds.notes`. Review the shared billing templates for the actual payment model.
The authentication text currently describes Auth0, which all three apps use.
Verify each app's data collection and legal terms before treating these pages as
launch-ready policies.

Owner details shared by every page (name, support email, jurisdiction) live under `owner:` in `_config.yml`.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

## Enabling GitHub Pages

Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main` / `(root)`.

> The legal pages are generic templates, not legal advice. Review them for your situation.
