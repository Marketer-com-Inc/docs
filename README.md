# Marketer documentation

Public product documentation for [Marketer](https://www.marketer.com), built with [Mintlify](https://mintlify.com/docs).

## Local development

From the repository root:

```bash
npx mint dev
```

The local site opens at `http://localhost:3000` unless another port is selected.

## Validation

Run the same checks before opening a pull request:

```bash
npx mint validate
npx mint broken-links --check-anchors --check-redirects --check-snippets
npx mint a11y
```

## Publishing

Mintlify is connected to the `main` branch of `Marketer-com-Inc/docs`. Pull requests receive preview builds when enabled in the Mintlify dashboard. A merge to `main` triggers the production deployment.

## Editorial source of truth

- Product behavior: `Marketer-com-Inc/marketer-new` on `origin/main`
- Live behavior: authenticated Marketer workspace walkthrough
- Page ownership and verification: `CONTENT-MAP.md`

Do not use the retained `sources/**` marketing scrape as evidence for product behavior.
