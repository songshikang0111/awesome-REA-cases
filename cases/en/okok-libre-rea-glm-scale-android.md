# OKOK Libre: REA/GLM APK research leads to an offline Android scale client

Category: Applications and clients · REA
Record date: 2026-10-31
Stage: In progress

At 19:13:19 Beijing time on October 31, 2026, JYunth (@j_yunth) says an Ant Esports body-composition scale bought on Zepto was tied to the ad-heavy, slow OKOK International app. They report using REA plus GLM 5.3 on its roughly 50MB APK, extracting formulas and APIs and rebuilding it as OKOK Libre, with Opus 5.5 making the UI. They also allege the original app uploaded weight data to a Chinese server. Exfiltration and 'every formula/the same math' remain author claims: the original APK, traffic and comparative formulas were not inspected here.

Supplementary reading covered the complete README, main AndroidManifest and CI definition of JYunth/okok-libre at commit 093a337a86025c532e0afd21e86fd856c8c5c00a. Dated October 31 at 18:44:40 Beijing time, before the candidate, the commit credits Claude Opus 5.5 as co-author. The README requires Android 8.0 or newer and Bluetooth LE, supports classic, OKOKCloud and OKOKCloudV4, and explicitly leaves some other device families unimplemented. Scales may report only weight, provide impedance or calculate composition themselves; universal OKOK-device or metric compatibility is not established. Documentation lists multiple profiles, local trends, backups and spreadsheet export. Screenshots use a fictional demo household, not real health data.

The pinned main manifest declares neither INTERNET nor an advertising-ID permission and disables backups. This is static-file inspection, not a runtime audit of final merged APK permissions, networking or security. The README warns that manual backups are unencrypted and composition figures are estimates, not medical advice. The GPL-3.0 implementation and test source are public; CI defines unit tests and debug/release builds, but was not run here. A workflow file is not proof of passing tests. No dependencies were installed, APK downloaded, scale connected or reproduction performed. In-progress status, protocol coverage and unverified formula equivalence remain explicit.

Candidate snapshot: 0 likes, 14 views, 0 reposts. 50MB is the author's figure; engagement is not functional evidence.
Android 8.0+ and three protocols are pinned-documentation scope; compatibility and body-composition accuracy were not tested.

## Sources

- [JYunth's REA/GLM/Opus scale-client report, October 31, 2026](https://x.com/i/status/2116488683188887716)
- [Supplementary pinned README: protocol coverage and privacy limits, October 31, 2026](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/README.md)
- [Supplementary pinned main AndroidManifest: static permissions, October 31, 2026](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/app/app/src/main/AndroidManifest.xml)
- [Supplementary pinned CI definition, not proof of passing tests, October 31, 2026](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/.github/workflows/ci.yml)

[中文](../okok-libre-rea-glm-scale-android.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
