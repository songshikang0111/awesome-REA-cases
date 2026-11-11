# Rental LG TVs: Kevin Theo uses Claude for welcome screens and Pi resets, finding persistent PlayReady login state

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: In progress

At 17:17:25 Beijing time on November 9, 2026, Kevin Theo (@kevintheo) reports three LG TVs in a holiday rental displaying guests' names, six languages, Wi-Fi QR codes, weather and local tips on-device. LG no longer updates the firmware, and he uses a root path supplied by webOS Homebrew. After stays, a Raspberry Pi reportedly resets each TV in two to three minutes, logging out Netflix, YouTube and Prime Video. Netflix remained logged in after application data was deleted until its hidden PlayReady store was also cleared. Investigating that concrete residual state is the case's research value; it does not establish DRM defeat or recovery of its cryptography.

The author explicitly says he decided and tested every version on the TVs; Claude Code wrote code and Codex, GLM, Muse and Grok reviewed it. He reports 38 findings on the public version on November 7, with 29 confirmed and fixed, each backed by a test that first failed. These are the author's project-QA counts, not 29 independently verified vulnerabilities. An earlier supplementary author reply at 17:29:09 says the public template contains the TV app, Pi component, tests and AGENTS.md under MIT with sample data. Retrieval confirms wording only; no exact repository, code or tests were obtained. The reply is contextual evidence, not an additional candidate.

A new secondary candidate at 07:36:54 Beijing time on November 11 adds reported testing on webOS 4.10 and 5.6, with rooting limited to firmware listed by Homebrew. The Pi reportedly pulls guest data from Smoobu or a JSON file hourly, plus Open-Meteo weather. The TV app refreshes every five minutes and still displays if the Pi is down. After checkout the Pi wakes each TV, deletes and checks streaming logins, reboots and turns it off. The alternative was three Google TV boxes plus kiosk licenses. These are secondary additions about architecture, versions and motivation; source and original tests were not obtained. They establish neither support for arbitrary LG firmware nor fresh offline information or complete credential removal.

The author warns that rooted, unpatched TVs must be on a network inaccessible to guests. LG models, full reset coverage and cross-application re-login checks remain unchecked. Two to three minutes is self-reported, not a security guarantee. Homebrew's existing root capability is not attributed as a new Claude discovery. REA is unmentioned. This collection connected no device, deleted no data and executed no project code.

Original sealed candidate: 1 like, 135 views, 0 reposts. Three TVs, six languages, two to three minutes per TV and 38/29 findings are author reports.
New November 11 candidate: 0 likes, 34 views, 0 reposts. webOS 4.10/5.6, hourly/five-minute refreshes and offline display are secondary claims, not independently checked.

## Sources

- [Kevin Theo's three-LG-TV welcome screens, resets and PlayReady investigation, November 9, 2026](https://x.com/i/status/2119721007988593136)
- [Supplementary author reply on the public template, AGENTS.md and tests, November 9, 2026 at 17:29:09 Beijing time](https://x.com/i/status/2119723960258465793)
- [New secondary candidate: webOS versions, Smoobu and Pi/TV refresh workflow, November 11, 2026](https://x.com/i/status/2120299691774550312)

[中文](../kevin-theo-lg-webos-rental-reset-playready.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
