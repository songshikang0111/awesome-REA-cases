# Claude Android and Sift: version-specific fields, not recovered KYC logic

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-17
Stage: Related project

At 19:58:10 Beijing time on October 29, 2026, Qian Duoduo (@Peterxvip) relays Sift anti-fraud research in Claude's Android package, claiming SIM country, carrier, interface IP and installed-app-list collection and reporting before login. Retrieval then confirmed only the relayer and text, without an original researcher, build, hash, code locations, permissions, OS revision or traffic evidence.

A new candidate at 16:28:22 on November 17 says an independent GitHub audit targets APK 1.260930.20, with code reading ANDROID_ID, SIM country and carrier, enumerating network-interface addresses and recording Sift traffic during cold start before login. The original repository and traffic records were not read, so this remains secondhand evidence. The new post does not repeat installed-app-list collection; not every older field is assigned to this build.

The new candidate distinguishes getSimCountryIso from getNetworkCountryIso: a Chinese SIM roaming in Japan can return CN and JP respectively. It saw evidence for SIM-country collection, not transmission of both country values. Local IPv6 can differ from a VPN exit, so an exit IP does not prevent local-field access; this does not establish the cause of a ban or KYC event. Verification after mobile login is anecdotal, while Sift's influence on Anthropic's risk decisions, weights and thresholds is unknown. Desktop clients also have telemetry; neither desktop safety nor inevitable Android KYC is promised. The post calls for independent reproduction on newer builds and controlled verification outcomes.

This Android target remains distinct from desktop-client research and is recorded as related AI-client work. Neither batch says AI performed the reversing, so rea remains unknown. Static SDK presence does not establish complete transmission of every field. Without the original audit, hash or call chain, this collection did not execute the APK, access identifiers or account configuration, or capture user communications. No identity-cleanup, ban-prevention or detection-evasion guarantee is offered.

October 29 candidate: 0 likes, 3 views, 0 reposts. No APK or traffic inspection here; AI assistance and banning causality are unknown.
November 17 sealed candidate: 0 likes, 163 views, 0 reposts, 0 replies. The build and cold-start traffic are secondhand reports.

## Sources

- [Qian Duoduo relays Claude Android Sift and field research, October 29, 2026](https://x.com/i/status/2115775197496365511)
- [Candidate supplement: 1.260930.20, SIM fields and KYC limits, November 17, 2026 at 16:28:22 Beijing time](https://x.com/i/status/2122607766976205099)

[中文](../claude-android-sift-secondary-analysis-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
