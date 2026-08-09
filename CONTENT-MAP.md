# Marketer documentation content map

Internal release ledger. Mintlify excludes this file from the public site.

- Product baseline: `Marketer-com-Inc/marketer-new` `origin/main` at `f3f5393a899bac988ee50ed204088e381bac3b5f`
- Documentation issue: `MAR-2142`
- Last audit date: 2026-08-09
- Owner: Product documentation
- Live verification account: `ashmit@marketer.com`

Status vocabulary:

- **GA** — documented as supported for customers with the required role, plan, and provider access.
- **Beta** — visible in product but explicitly labeled Beta.
- **Conditional** — visibility or mutation rights depend on role, plan, workspace count, or configured integration.
- **Editorial** — request pattern or explanation rather than a discrete product surface.

## Get Started

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/get-started/introduction` | All users | GA | `/dashboard` | `frontend/components/sidebar/app-sidebar-navigation.tsx` | Verified 2026-08-09 | Home |
| `/get-started/quickstart` | New users | GA | `/get-started`, `/dashboard` | `frontend/app/get-started/page.tsx`; signup onboarding components | Verified 2026-08-09 | Integrations; Home; completed result |
| `/get-started/workspace-and-data` | New users, owners | Conditional | `/get-started`, `/dashboard/settings/integrations` | signup onboarding runtime; integration registry | Integration states verified 2026-08-09 | Home; Integrations; connected Meta |
| `/get-started/first-task` | New users | GA | `/dashboard` | dashboard page and chat composer | Real read-only task completed; deterministic task states verified 2026-08-09 | Home; active task; completed result |
| `/get-started/review-result` | All users | Editorial | `/dashboard` | chat result and analytics surfaces | Real result reviewed 2026-08-09 | Completed result |
| `/get-started/next-steps` | Activated users | Conditional | `/dashboard` | `frontend/lib/sidebar/getting-started.ts` | Checklist and product routes verified 2026-08-09 | Completed result |

## Essential Guidelines

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/essential-guidelines/context-and-grounding` | All users | Editorial | `/dashboard` | chat context picker; Knowledge surfaces | Knowledge and Skills verified 2026-08-07 | Not required |
| `/essential-guidelines/effective-requests` | All users | Editorial | `/dashboard` | chat composer and task model | Real read-only task completed 2026-08-07 | Not required |
| `/essential-guidelines/sources-and-freshness` | Analysts | Conditional | `/dashboard/analytics`, integrations | integration and analytics surfaces | Live statuses and sync coverage verified 2026-08-07 | Not required |
| `/essential-guidelines/review-results` | All users | Editorial | Result-dependent | result and approval surfaces | Real result reviewed 2026-08-07 | Not required |
| `/essential-guidelines/approvals-and-autonomy` | Owners, Admins, approvers | Conditional | `/dashboard/awaiting-action`, settings | settings nav, guardrails, autonomy, awaiting-action pages | Verified 2026-08-07 | Not required |

## Working with Marketer

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/working-with-marketer/overview` | All users | GA | `/dashboard` | sidebar navigation; dashboard page | Verified 2026-08-09 | Home |
| `/working-with-marketer/home-and-composer` | All users | GA | `/dashboard` | Home page, composer, context picker, and agent picker | Home and composer verified read-only 2026-08-09 | Home |
| `/working-with-marketer/navigation-and-quick-actions` | All users | Conditional | `/dashboard` | sidebar navigation, Quick actions, recents, and tool preferences | Current sidebar and Quick actions verified read-only 2026-08-09 | Sidebar; Quick actions |
| `/working-with-marketer/chat-and-context` | All users | GA | `/dashboard` | chat composer and context picker | Real read-only task completed 2026-08-09 | Home; completed result |
| `/working-with-marketer/answers-tasks-and-proposals` | All users | Conditional | `/dashboard`, task routes | chat response, task, question, and proposal components | Source-aligned branches and deterministic task states verified 2026-08-09 | Active task; completed result |
| `/working-with-marketer/questions-and-approvals` | Requesters, approvers | Conditional | chat and `/dashboard/awaiting-action` | question, run-proposal, tool-approval, and awaiting-action components | Source-aligned decision boundaries verified 2026-08-09 | Not required |
| `/working-with-marketer/tasks-and-activity` | All users | GA | `/dashboard`, `/dashboard/activity` | task/activity components | Task rail and result verified 2026-08-09 | Active task; completed result |
| `/working-with-marketer/task-control-and-recovery` | All users | Conditional | task routes, `/dashboard/activity` | task controls, waiting states, cancellation, retry, and output components | Source-aligned task states verified 2026-08-09 | Not required |
| `/working-with-marketer/specialists` | All users | Conditional | `/dashboard` | specialist catalog and picker | Deterministic specialist and nested-run states verified 2026-08-09 | Workbench overview; specialist detail |
| `/working-with-marketer/awaiting-action` | Approvers | Conditional | `/dashboard/awaiting-action` | awaiting-action page and approval components | Proposal decision state verified 2026-08-09 | Not required |
| `/working-with-marketer/chats-and-tasks` | All users | GA | `/dashboard/chat/all` | combined history page, tabs, search, and row routing | Current production controls verified read-only 2026-08-09 | Chats and tasks controls |
| `/working-with-marketer/history-and-notifications` | All users | GA | `/dashboard/chat/all`, `/dashboard/notifications` | sidebar navigation; chat and notification pages | Verified 2026-08-09 | Home |

## Product Guides

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/product-guides/campaigns` | Media buyers | Conditional | `/dashboard/campaigns` | campaigns pages and components | Five deterministic campaign states verified 2026-08-09 | Overview; saved view; channel choice; Meta setup; drafts |
| `/product-guides/analytics` | Analysts, operators | Conditional | `/dashboard/analytics`, `/dashboard/settings/conversion-metrics`, `/dashboard/workflows?kind=reports` | analytics, conversion-metric, and reports surfaces | Performance, controls, and syncing states verified 2026-08-09; Conversion metrics unavailable in live workspace pending migration | Overview; controls; syncing |
| `/product-guides/analytics-performance-and-views` | Analysts, operators | Conditional | `/dashboard/analytics` | Performance cards, measurement controls, breakdowns, and custom views | Deterministic Analytics states and current source verified 2026-08-09 | Overview; controls; syncing |
| `/product-guides/analytics-creative-performance` | Creative analysts | Conditional | `/dashboard/creatives` | creative-performance filters, cards, breakdowns, and placement views | Authenticated owning surface and current source verified read-only 2026-08-09 | Creative performance |
| `/product-guides/creatives` | Creative teams | Conditional | `/dashboard/creatives`, `/dashboard/briefs`, `/dashboard/studio/ads`, `/dashboard/creative-library` | creative performance, briefs, Studio, and Creative Assets components | Four owning surfaces and deterministic Creative Pipeline verified read-only 2026-08-09 | Performance; Briefs; Studio; Creative Assets; Creative Pipeline detail |
| `/product-guides/creatives-briefs` | Creative teams | Conditional | `/dashboard/briefs` | brief hierarchy, avatars, ad briefs, generation, and launch handoff | Authenticated owning surface and current source verified read-only 2026-08-09 | Briefs |
| `/product-guides/creatives-studio` | Creative teams | Conditional | `/dashboard/studio/ads` | Studio composer, generation controls, version review, and save handoff | Authenticated owning surface and current source verified read-only 2026-08-09 | Studio |
| `/product-guides/creatives-assets` | Creative teams | Conditional | `/dashboard/creative-library` | Creative Assets filters, labels, uploads, sync, and detail controls | Authenticated owning surface and current source verified read-only 2026-08-09 | Creative Assets |
| `/product-guides/workflows` | Operators | Conditional | `/dashboard/workflows` | workflows page and configuration components | Workflow library and approval boundary verified read-only 2026-08-09 | Workflow library |
| `/product-guides/workflows-reports-alerts-and-runs` | Operators | Conditional | `/dashboard/workflows` | Autopilot, report and alert setup, workflow register, and run detail | Current production library verified read-only 2026-08-09; dynamic runs source-verified | Workflow library |
| `/product-guides/knowledge-and-skills` | All users, owners | Conditional | `/dashboard/knowledge-base`, `/dashboard/knowledge-base/skills` | knowledge and skills surfaces | Verified read-only 2026-08-07 | Saved-context retrieval in task progress |
| `/product-guides/knowledge-sources` | All users, owners | Conditional | `/dashboard/knowledge-base` | source ingestion, routing, retrieval, and saved-context components | Owning surface and current source verified read-only 2026-08-09 | Saved-context retrieval in task progress |
| `/product-guides/knowledge-skills` | All users, owners | Conditional | `/dashboard/knowledge-base/skills` | Skills library, import, promotion, pinning, and evaluation components | Current production controls verified read-only 2026-08-09 | Skills controls |
| `/product-guides/products` | Commerce teams | Conditional | `/dashboard/products` | product catalog and detail pages | Verified read-only 2026-08-09 | Integrations prerequisite |
| `/product-guides/products-catalog-and-enhancement` | Commerce teams | Conditional | `/dashboard/products`, product detail, Studio | catalog, product detail, sync, handoff, and enhancement components | Current production catalog controls verified read-only 2026-08-09 | Product catalog controls |
| `/product-guides/campaigns-inspect-and-manage` | Media buyers | Conditional | `/dashboard/campaigns` | campaign filters, levels, saved views, table, and live actions | Deterministic campaign states and current source verified 2026-08-09 | Saved view |
| `/product-guides/campaigns-meta-build` | Media buyers | Conditional | Meta campaign builder | Meta setup, tree builder, validation, review, and publish components | Deterministic Meta setup and current source verified 2026-08-09 | Meta setup |
| `/product-guides/campaigns-google-build` | Media buyers | Conditional | Google campaign builder | Google objective, type-specific builders, validation, review, and publish components | Current source verified; provider-dependent states not mutated | Channel choice |
| `/product-guides/campaigns-drafts-and-launches` | Media buyers, approvers | Conditional | `/dashboard/campaigns` | draft drawer and launch-progress components | Deterministic draft and launch states verified 2026-08-09 | Drafts |

## Integrations

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/integrations/overview` | Owners, Admins, Members | Conditional | `/dashboard/integrations` | `frontend/components/integrations/integration-registry.tsx` | Directory states verified 2026-08-09 | Integration directory |
| `/integrations/meta-ads` | Owners, Admins | GA | `/dashboard/settings/integrations/meta` | registry, setup guide, Meta connect/disconnect components | Connected and reconnect-needed states verified 2026-08-09 | Connected provider detail |
| `/integrations/google-ads` | Owners, Admins | GA | `/dashboard/settings/integrations/google-ads` | registry, setup guide, Google Ads connect/disconnect components | Connected, selection, and reconnect states verified 2026-08-09 | Account-selection step |
| `/integrations/google-ads-auto-apply` | Owners, Admins | Conditional | `/dashboard/settings/integrations/google-ads` | recommendation-subscription controls and account read-back | Production section verified read-only 2026-08-09; subscription settings not mutated | Not required |
| `/integrations/shopify` | Owners, Admins | GA | `/dashboard/settings/integrations/shopify` | registry, setup guide, Shopify connect/disconnect components | Connected state verified 2026-08-07 | Not required |
| `/integrations/google-analytics-4` | Owners, Admins | GA | `/dashboard/settings/integrations/ga4` | registry, setup guide, GA4 connect/disconnect components | Connected state verified 2026-08-07 | Not required |
| `/integrations/slack` | Owners, Admins | GA | `/dashboard/settings/integrations/slack` | Slack app/setup/disconnect components | Connected state verified 2026-08-07 | Not required |
| `/integrations/beta` | Beta users | Beta | provider-specific settings routes | integration registry | Microsoft, OpenAI, and Triple Whale routes verified 2026-08-07 | Not required |
| `/integrations/troubleshooting` | Owners, Admins | Conditional | provider-specific settings routes | OAuth bridge and cancellation/error components | Live state mismatch captured 2026-08-07 | Not required |

## Workspace and Admin

| Page | Audience | Status | App route | Code/config source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- | --- |
| `/workspace-admin/overview` | Owners, Admins | Conditional | `/dashboard/settings/profile` | `frontend/components/settings/settings-nav-items.ts` | Verified 2026-08-07 | Not required |
| `/workspace-admin/workspace-switching` | Multi-workspace users | Conditional | workspace switcher | workspace selector, access policy, and navigation state | Current production switcher and source verified read-only 2026-08-09 | Not required |
| `/workspace-admin/account-overview` | Multi-workspace Owners, Admins | Conditional | `/dashboard/account/overview` | account eligibility, rollups, billing, users, and MCP sections | Ineligible-account redirect verified live 2026-08-09; eligible tabs source-verified and not mutated | Not required |
| `/workspace-admin/profile-and-authentication` | All users | GA | `/dashboard/settings/profile`, `/dashboard/settings/authentication` | settings pages and navigation | Profile and signed-in email verified 2026-08-07 | Not required |
| `/workspace-admin/mcp-connect` | All users with access | Conditional | `/dashboard/settings/api-keys` | MCP connect page and setup checklist | Verified read-only 2026-08-07 | Not required |
| `/workspace-admin/brand-and-autofills` | Owners, Admins, Members | Conditional | `/dashboard/settings/branding`, `/dashboard/settings/autofills` | settings pages and navigation | Brand kit, competitor watchlist, and all four Autofills areas verified read-only 2026-08-09 | Not required |
| `/workspace-admin/members-and-roles` | Owners, Admins | Conditional | `/dashboard/settings/team` | team management and membership policy | Verified read-only 2026-08-07 | Not required |
| `/workspace-admin/guardrails-and-autonomy` | Owners, Admins | Conditional | `/dashboard/settings/guardrails`, `/dashboard/settings/autonomy` | settings pages and policy components | Verified read-only 2026-08-07 | Not required |
| `/workspace-admin/audiences` | Owners, Admins, Members | Conditional | `/dashboard/settings/audience-segments` | audience settings pages | Audience segments, New segment, and Existing/Engaged role controls verified read-only 2026-08-09 | Not required |
| `/workspace-admin/custom-audiences` | Owners, Admins, Members | Conditional | `/dashboard/settings/custom-audiences` | Meta audience list, creation flows, terms, and processing states | Production route verified read-only 2026-08-09; no provider audience created | Not required |
| `/workspace-admin/conversion-metrics` | Owners, Admins | Conditional | `/dashboard/settings/conversion-metrics` | conversion selection, labels, order, and primary-metric controls | Unavailable-state verified live 2026-08-09; available state source-verified | Not required |
| `/workspace-admin/notifications-and-billing` | All users; billing roles | Conditional | notification and subscription settings routes | settings navigation and pages | Verified read-only 2026-08-07 | Not required |
| `/workspace-admin/security-and-troubleshooting` | All users | Editorial | settings and integration routes | authentication, role, and integration error surfaces | Authentication reset/global-sign-out controls and layered recovery surfaces verified read-only 2026-08-09 | Not required |

## Templates and Use Cases

| Page | Audience | Status | Product evidence | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- |
| `/templates-use-cases/overview` | All users | Editorial | Links to documented product surfaces | Pending | Not required |
| `/templates-use-cases/analyze-performance` | Analysts | Editorial | Analytics and chat | Pending | Not required |
| `/templates-use-cases/diagnose-change` | Analysts | Editorial | Analytics, integrations, Knowledge | Pending | Not required |
| `/templates-use-cases/creative-brief` | Creative teams | Editorial | Briefs, Knowledge, Creatives | Pending | Not required |
| `/templates-use-cases/safe-campaign-launch` | Media buyers, approvers | Conditional | Campaign drafts, guardrails, approvals | Pending | Not required |
| `/templates-use-cases/recurring-report` | Operators | Conditional | Workflows and delivery configuration | Pending | Not required |
| `/templates-use-cases/reusable-skill` | All users | Conditional | Knowledge and Skills | Pending | Not required |

## Release Notes

| Page | Audience | Status | Source | Live verification | Screenshot |
| --- | --- | --- | --- | --- | --- |
| `/release-notes/overview` | All users | GA | Merged customer-facing releases and documentation PRs | Published and verified 2026-08-07 | Not required |

## Authenticated verification evidence

- Chrome profile: `ashmit@marketer.com`, confirmed before product, screenshot, and Mintlify work.
- Focused-guide live pass: current Products, Skills, Workflows, Chats and tasks, sidebar, Quick actions, Branding & Brand Profile, Autofills, Audience segments, Custom audiences, Authentication, Google Ads auto-apply, and conversion-metric surfaces were inspected read-only on 2026-08-09. The live account correctly redirected the ineligible Account overview route to the workspace dashboard. No provider, audience, workflow, billing, access, authentication, or account setting was changed.
- Real read-only task: `/dashboard/chat/99723720-ef00-4169-a05a-8b2d133accb3` on 2026-08-07.
- Exact result excerpts: “Shopify: Connected and active.” “Slack: Connected and active.” “Meta: Not connected.” “Google Ads: Not connected.” “No connection, profile, campaign, approval, or account setting was changed.”
- Reconciliation evidence: the same workspace's visible provider UI showed **Reconnect needed** for Meta Ads and Google Ads, including last-sync and coverage details. Public guidance now preserves both observations and blocks connection changes until the intended account is confirmed.
- Conversion metrics: the live settings route showed “Conversion metrics aren't available yet” and identified the unapplied `workspace_conversion_metrics` migration. Public guidance treats the surface as conditional without claiming a workspace-specific rollout mechanism.
- Product-flow captures: the published set uses deterministic, network-free UI states inspected through authenticated production `/dev` routes on 2026-08-09. Authenticated production crops additionally cover Creatives, Briefs, Studio, Creative Assets, navigation, Quick actions, Chats and tasks, Products, Skills, and Workflows. Published crops omit admin controls, user identifiers, provider resource IDs, customer content, customer metrics, and customer-only details.
- Deterministic screenshot sources: `/dev/home`, `/dev/apps`, `/dev/analytics`, `/dev/campaigns`, `/dev/result-block/chat-parity`, and `/dev/result-block/workbench-parity`. Every capture uses production components or the route's documented source fixture rather than a synthetic mockup.
- Mintlify preview: `https://marketer-com-ashmit-mar-2142-marketer-docs.mintlify.site/`; representative pages and legacy redirects verified on 2026-08-07.
- Focused-guide preview: `https://marketer-com-ashmit-mar-2142-deep-product-guides.mintlify.site/`; five representative focused guides and their current content verified before merge on 2026-08-09.
- Production: merge commit `2202a37230a7cc36a0ffe1166cd745e91620d9ab` deployed successfully to `https://marketer-com.mintlify.site/`; home, representative guides, feedback, and legacy redirects verified on 2026-08-07.
- Focused-guide production: PR `#4`, merge commit `9678632d15b8fefcac660588df189e42a011ee19`, and served version `dpl_2aZXKXcCsy1h7hFSCxdUkNT2EkoS` are live on `https://docs.marketer.com`. Home/composer, Google campaign build, Products, Conversion metrics, Google Ads auto-apply, and the 176,921-byte Workflow library PNG were verified twice after deployment on 2026-08-09.
- Access decision: full Mintlify authentication was disabled with explicit approval on 2026-08-09; the default Mintlify domain returns public pages without a login redirect.
- Custom domain: `docs.marketer.com` is registered in Mintlify, its two validation TXT records and DNS-only CNAME resolve publicly, and Mintlify serves a valid certificate and fresh documentation at the custom domain.

## Product screenshot ledger

| Asset family | Authenticated source | Public use | Sanitization |
| --- | --- | --- | --- |
| Home | `/dev/home?view=filled&theme=light` | Orientation, workspace context, request entry | Deterministic sample workspace; no user or provider identifiers |
| Task states | `/dev/result-block/chat-parity` fixture scenarios | Active work, proposal, completed result | Cropped to the production chat surface; admin banner and workspace identity removed |
| Specialist states | `/dev/result-block/workbench-parity` fixture scenarios | Specialist overview and nested Creative Pipeline result | Cropped to the production workbench surface; admin banner and workspace identity removed |
| Integrations | `/dev/apps` directory and provider-detail scenarios | Connection prerequisites and setup state | Provider resource IDs excluded from published crops |
| Analytics | `/dev/analytics` overview, controls, and syncing scenarios | Measurement frame, source coverage, and sync state | Deterministic source fixtures; no live account identifiers |
| Campaigns | `/dev/campaigns` overview, view, create, setup, and draft scenarios | Campaign inspection and draft-to-review flow | Deterministic source fixtures; no live campaign or account identifiers |
| Creative production | Authenticated QA captures of `/dashboard/creatives`, `/dashboard/briefs`, `/dashboard/studio/ads`, and `/dashboard/creative-library`, reconciled with `origin/main` | Performance frame, brief hierarchy, Studio composer, and asset library | UI-only crops remove workspace rail, admin banner, customer records, creative content, and account identifiers |
| Navigation | Authenticated production sidebar and Quick actions | Current entry points, hidden-surface access, recents, and customizable tools | Crops exclude workspace identity, recents, customer content, and account controls |
| Chats and tasks | Authenticated production `/dashboard/chat/all` | Combined-history tabs, search, and new-chat entry | Header-only crop excludes conversation titles, timestamps, and workspace identity |
| Products | Authenticated production `/dashboard/products` | Catalog scope, layout, sort, resync, search, and add-product controls | Toolbar-only crop excludes product records, counts, sales values, and workspace identity |
| Knowledge and Skills | Authenticated production `/dashboard/knowledge-base/skills` | Skills explanation and import entry | Header-only crop excludes Skill records, results, and workspace identity |
| Workflows | Authenticated production `/dashboard/workflows` | Library, Autopilot request entry, and current report and alert cards | Crop excludes workspace rail, customer workflows, run history, identifiers, and metrics |

## Release gates

- [x] Canonical docs repository and Mintlify `main` branch connection confirmed.
- [x] GitHub app installed for automatic updates.
- [x] All navigable pages pass Mintlify validation, links, and accessibility checks.
- [x] Representative customer flows match the authenticated app.
- [x] Pull request preview is reviewed.
- [x] Production deployment and redirects are verified.
- [x] Mintlify add-ons reviewed: thumbs feedback and automatic related topics enabled; broken-link CI set to Blocking; authenticated PR previews already enabled.
- [x] Public-access decision is recorded and the default Mintlify domain is public.
- [x] `docs.marketer.com` is registered in Mintlify with exact DNS instructions recorded.
- [x] Cloudflare TXT and CNAME records are created and validated; `docs.marketer.com` serves a valid certificate and current content.
- [x] The screenshot-driven product-flow release passed validation, strict links, accessibility, local visual review, PR review, merge, and production verification.
- [x] The focused feature-guide release passes source review, Mintlify validation, strict links, accessibility, PR review, merge, and production verification.
