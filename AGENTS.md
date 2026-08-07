# Marketer documentation instructions

## About this project

- This is the public Marketer product documentation built with Mintlify.
- Configuration lives in `docs.json`; pages are MDX with YAML frontmatter.
- The canonical product source is `Marketer-com-Inc/marketer-new` on `origin/main`.
- The public site explains customer-facing behavior. It is not a marketing-site mirror or an internal engineering manual.

## Terminology

- Use **workspace** for a customer's working environment.
- Use **connected account** or the provider name for data sources.
- Use **Marketing Agent** for the unified agent and **specialist** for a focused agent selected in chat.
- Use **Creatives**, **Briefs**, **Studio**, and **Assets**. Do not use the retired Ember product name.
- Use the exact UI label **Awaiting action** for requests that need review or input.
- Use **Owner**, **Admin**, **Member**, and **Viewer** for workspace roles.
- Label Microsoft Ads, OpenAI Ads, and Triple Whale as **Beta** wherever they appear.

## Style

- Use active voice and second person.
- Lead with the outcome, then explain the concept or steps.
- Keep sentences concise and headings in sentence case.
- Bold UI labels. Use code formatting for commands, paths, and code references.
- Prefer plain Markdown. Use Mintlify components only when they improve scanning or clarify sequence, status, or risk.
- Avoid marketing language, guarantees, unsourced statistics, and vague claims such as “real time.” State the data source and freshness context instead.

## Product truth

- Verify behavioral claims against both production code/config and an authenticated workspace walkthrough.
- Treat navigation, permissions, plans, Beta status, and data freshness as changeable product facts.
- If a claim is not verified, omit it or leave a clear MDX TODO comment.
- Keep screenshots sanitized, current, locally stored, and paired with descriptive alt text.

## Content boundaries

- Document customer-facing app surfaces only.
- Do not document internal admin, BI, designer, developer, private API, feature-flag, runtime, or job-system details.
- Do not publish unsupported integrations or generic connector/API promises.
- Do not promise universal autonomy, universal Slack approval, guaranteed outcomes, or fixed setup times.
- Keep marketing case studies, industry pages, and scraped website copy outside the product documentation.

## Verification

Before publishing, run:

```bash
mint validate
mint broken-links --check-anchors --check-redirects --check-snippets
mint a11y
```

Also verify the changed flows in the authenticated Marketer workspace and update `CONTENT-MAP.md` with the result.
