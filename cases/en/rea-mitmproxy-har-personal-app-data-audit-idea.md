# Inspecting data sent by one's own apps: a mitmproxy HAR-to-Claude/REA audit idea

Category: Applications and clients · REA
Record date: 2026-11-13
Stage: Needs verification

At 23:45:48 Beijing time on November 13, 2026, a poster proposes a personal-app privacy audit: route one app on one's own machine through mitmproxy, save the session as a HAR file, configure REA, then ask Claude Code to read session.har and list requests carrying personal data and the code sending them. The aim is to identify what left, where it went and which program component was responsible, rather than merely noticing network activity. This is a usage idea with explicit inputs and intended outputs, not a report of an audited app.

The post predicts exposure greater than data leaks but supplies no app name, HAR, binary, capture scope, code-locator output or measurements. HAR describes captured HTTP exchanges; it does not automatically contain exact source code or binary call chains. Attributing requests to code needs corresponding programs, stacks or other evidence, while capture gaps, encryption and handling personal data are not addressed in the post. Not all communication is a privacy leak, and the sixty-second promotion is not a measured duration. This collection did not configure a proxy, install certificates, collect personal data, execute REA or verify the pipeline. Retained as an unverified proposal.

Candidate snapshot: 5 likes, 114 views, 0 reposts, 0 replies. No audit report; precise code attribution and sixty seconds are unverified.

## Sources

- [Candidate: personal-app audit idea using mitmproxy HAR and Claude/REA, November 13, 2026 at 23:45:48 Beijing time](https://x.com/i/status/2121268300499874190)

[中文](../rea-mitmproxy-har-personal-app-data-audit-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
