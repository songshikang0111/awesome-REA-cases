# From an APK to its backend: Tech Athletes relays NICT's A2B investigation and an AI-cost claim

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-24
Stage: Needs verification

At 21:26:40 Beijing time on November 24, 2026, Tech Athletes (@IT_makesUsHappy) describes App-to-Backend (A2B) attacks: start with apps publicly available on Google Play in Japan, decompile them, extract API hosts, endpoints, parameters and responses, then tailor an attack to each backend. The writer says AI makes this analysis cheaper, mentioning SSRF, remote code execution, SQL injection and IDOR/BOLA object-authorization failures. The purpose is to explain why a hardened client cannot replace server-side authorization, not to publish exploitation code for a named app.

The post attributes the observations to NICT's October 13, 2026 report and relays categories from a JPCERT/CC update on October 23: endpoints/keys in public apps, interfaces unreachable through the UI, role or account operations, blind NoSQL injection and API keys leaked from other systems. It recommends inventorying new and old APIs and test environments, reviewing logs from August, checking authorization and injection, shutting unused interfaces, rate limiting and rotating exposed keys. These are dates of earlier material cited by the writer, not the date of this window's candidate.

Supplementary retrieval confirms attribution. The institutional originals, affected app names, models, prompts, analysis records and cost comparisons were not obtained. Actual AI use in a particular intrusion cannot be confirmed, nor can the entire leak wave be attributed to AI. This retains only the writer's relayed research path and cost claim. No backend requests, vulnerability tests or APK execution were performed. REA is unmentioned; status remains unverified.

Sealed candidate: 0 likes, 48 views, 0 reposts, 0 replies. Reduced AI-analysis cost is the poster's statement, not a quantified experiment.

## Sources

- [Tech Athletes relays A2B research, November 24, 2026, citing NICT on October 13 and JPCERT/CC on October 23](https://x.com/i/status/2125219553592685034)

[中文](../nict-a2b-ai-assisted-mobile-backend-analysis-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
