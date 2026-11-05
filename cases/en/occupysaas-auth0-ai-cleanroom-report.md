# zeroauthy: OccupySaaS's Auth0-compatible identity server, with full replacement still a goal

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-06
Stage: In progress

At 09:14 Beijing time on November 3, 2026, an English post says laid-off engineers formed OccupySaaS to build AI-assisted clean-room replacements for Auth0 and Salesforce, under Apache-2.0 and with drop-in compatibility. This record covers only Auth0 identity services. Employment history, AI's work share and the motive of replacing former employers come from the post and were not independently established.

The occupysaas organization identifies the zeroauthy repository. Its README was read at commit 5d1c30c1ac7c90d88307c1958af7d7fd20ef0d54, dated November 2 at 14:56 Beijing time, before this round. It describes a self-hostable Auth0 Authentication/Management API implementation from public documentation and open standards, listing discovery/JWKS, authorization code with PKCE, refresh tokens, a console, organizations and event streams. The project reports testing bounded paths with auth0-spa-js, auth0-react, nextjs-auth0 and auth0-cli.

The README claims OpenID Foundation certification for the Basic, Config and Form Post OP profiles, approved October 30; the directory was not separately checked here. Even confirmed certification would not establish all Auth0 features. The project remains early, with MFA, passwordless/phone flows, more enterprise protocols and production hardening on the roadmap, plus migration exclusions. AI attribution comes from the candidate; features and tests come from the project, neither being independent reproduction.

A new candidate at 00:46:39 on November 6 reports a November 4 v1.0.0-rc.1 release, with login, tokens, multitenancy, binaries and container images. It describes rewriting from public documentation and standards and validating with public SDKs, rather than stealing code or decompiling. It reports 836 commits in 22 days, Claude co-author attribution in 64% of commit lines, 390 Opus 5.5 commits, 150,000 Go lines and 120,000 test lines. Commit lines, commit counts and code lines are different measures. No statistics script, matching commit set or fresh release-package verification was obtained, so these do not measure AI's work share, quality or complete compatibility. The post explicitly retains an early-preview, non-production warning and missing passkey/SAML support; new numbers do not override the older documentation's limits. No builds, SDK tests, logins or real identity credentials were used here. Apache-2.0 and clean-room remain project/post claims, not legal compliance findings.

November 3 shared candidate: 0 likes, 20 views, 0 reposts. OpenID certification is a project statement, not separately checked.
November 6 shared sealed candidate: 2 likes, 141 views, 0 reposts. The rc.1 and commit statistics are secondary reports, not independently validated.

## Sources

- [Report on OccupySaaS's AI Auth0/Salesforce rebuilding, November 3, 2026](https://x.com/i/status/2117425216573821238)
- [Supplementary pinned zeroauthy README, commit dated November 2, 2026, before the window](https://github.com/occupysaas/zeroauthy/blob/5d1c30c1ac7c90d88307c1958af7d7fd20ef0d54/README.md)
- [New report: ZeroAuthy rc.1 and Claude commit statistics, November 6, 2026 at 00:46:39 Beijing time](https://x.com/i/status/2118384508743389461)

[中文](../occupysaas-auth0-ai-cleanroom-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
