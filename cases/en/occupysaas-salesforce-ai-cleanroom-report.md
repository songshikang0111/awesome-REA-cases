# SalesCompel: OccupySaaS's Salesforce candidate explicitly remains non-production-ready

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-06
Stage: In progress

At 09:14 Beijing time on November 3, 2026, the OccupySaaS report also names a Salesforce CRM replacement, recorded separately from Auth0 identity services. Its AI, clean-room, Apache-2.0 and drop-in claims do not establish a complete Salesforce replacement or safe production migration.

The organization's salescompel README was read at commit 2aa326536f38768c24744079398966d325bb6589, dated October 22 at 01:10 Beijing time, before this round. It describes an initial tenant-isolated Go/PostgreSQL backend and Vue record workflow, with Account/Contact CRUD, describe, limited queries, external-ID upsert and provisioned bearer authentication. The UI preview uses synthetic data and keeps edits in memory without backend calls; unimplemented destinations are disabled and marked Planned.

The README's October 20 progress accepts an eleven-scenario reference baseline and bounded walking slices; Plan 16 records two local candidate-acceptance runs. However, no full-program milestone has a recorded exit-gate pass, Salesforce compatibility certification has not been performed and the candidate is explicitly not production-ready. Protocol, security, migration, automation and production verification remain substantial work. Roughly 185–350 additional plan equivalents is a scope estimate, not labor hours or a delivery date.

A new candidate at 00:46:39 on November 6 again identifies SalesCompel as OccupySaaS's Salesforce alternative, describing only account creation and contact reading, with substantial work before usability. Account creation may mean CRM Account records, not a complete user-registration system. The short retelling provides no pinned commit, demo or tests. It neither disproves the older README's bounded API scope nor transfers ZeroAuthy's rc.1, commit counts or code volume to SalesCompel. The project remains in progress and non-production-ready. No tests, CRM connections or customer data were used here. AI participation and the laid-off-team story come from candidates, not proof in the project documentation.

November 3 shared candidate: 0 likes, 20 views, 0 reposts. Documentation explicitly denies Salesforce compatibility certification; a reference baseline is not full candidate acceptance.
November 6 shared sealed candidate: 2 likes, 141 views, 0 reposts. The new summary is not a test, and ZeroAuthy's version and scale are not transferred.

## Sources

- [Report on OccupySaaS's AI Auth0/Salesforce rebuilding, November 3, 2026](https://x.com/i/status/2117425216573821238)
- [Supplementary pinned SalesCompel README, commit dated October 21 UTC, before the window](https://github.com/occupysaas/salescompel/blob/2aa326536f38768c24744079398966d325bb6589/README.md)
- [New report's SalesCompel account/contact stage, November 6, 2026 at 00:46:39 Beijing time](https://x.com/i/status/2118384508743389461)

[中文](../occupysaas-salesforce-ai-cleanroom-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
