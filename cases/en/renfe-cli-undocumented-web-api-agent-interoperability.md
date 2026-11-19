# Renfe CLI: web API research for agent-friendly Spanish train searches and delays

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-20
Stage: In progress

At 03:49:13 Beijing time on November 20, 2026, Luis González (@luisgonzaleznf) says Renfe CLI's core is reverse engineering Renfe's web APIs, with @hugojm_ building MCP for Claude, Instinct and other agents. Renfe is Spain's railway operator. The goal is avoiding a difficult website while retrieving trains, fares and delays and handing users to checkout. AI is not claimed to have performed the research itself; this is retained as interoperability for AI tools, with REA unconfirmed.

His November 19 introduction at 22:50:11 Beijing time and the README at November 19 UTC commit ac226de were read as supplementary evidence. Docs describe anonymous undocumented web API calls and JSON output, no account or user API key for searching, roughly 1,400 bundled stations and status from a public train map. They distinguish the legacy shop before January 25, 2027 from the newer shop afterward: legacy failures return an explicitly partial list, unknown delays are not zero and blocks/rate limits stop requests.

The docs report a November 17 legacy Madrid–Barcelona query yielding 24 trains from EUR 31.15 and a newer-system comparison of 22 trains matching the website. These are project checks, not live prices or reproduction here. Checkout and payment need additional browser interaction; account-free search does not imply unconfirmed autonomous payment. No installation, Renfe calls, passenger-data entry or purchase was performed here. MCP remains in progress in the candidate; a supplementary reply promising availability that night is not delivery evidence. Supplementary introduction and docs predate the strict window.

## Sources

- [Luis on web API research and MCP in progress, November 20, 2026](https://x.com/i/status/2123503882525454567)
- [Supplement: author's Renfe CLI introduction, November 19, 2026](https://x.com/i/status/2123428629560320247)
- [Supplement: README pinned to November 19 UTC commit](https://github.com/luisgonzaleznf/renfe-cli/blob/ac226dede6a5ad78543c8a7fd784e8f2b62fee00/README.md)

[中文](../renfe-cli-undocumented-web-api-agent-interoperability.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
