# JobBeacon docs

Customer-facing documentation for [JobBeacon](https://jobbeacon.app), built on [Mintlify](https://mintlify.com).

## Local preview

Install the Mintlify CLI:

```bash
npm i -g mint
```

Then from the repo root (where `docs.json` lives):

```bash
mint dev
```

The site is served at `http://localhost:3000`.

## Structure

- `docs.json` — site config (nav, branding, colors)
- `index.mdx` — landing page
- `quickstart.mdx` — 5-minute onboarding walkthrough
- `guides/` — product guides (adding companies, filters, notifications, sharing, billing, FAQ)
- `logo/`, `images/`, `favicon.svg` — brand assets

## Writing tips

- Active voice, second person ("you")
- Sentence case headings
- Bold for UI elements (e.g., **Add company**)
- Code formatting for URLs, paths, and field names

## Publishing

The Mintlify GitHub app deploys the default branch automatically — push to `main` and the site updates within a minute.

## Troubleshooting

- Dev server not starting? Run `mint update`.
- Broken links? Run `mint broken-links`.
