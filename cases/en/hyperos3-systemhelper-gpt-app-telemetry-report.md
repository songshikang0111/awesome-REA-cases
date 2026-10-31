# HyperOS 3 SystemHelper: MeT reports GPT findings on app lists and SIM-identifier payloads

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-31
Stage: Needs verification

At 20:16:14 Beijing time on October 31, 2026, MeT (@MeTerminator666) says friends received calls demanding removal of X and Telegram and therefore investigated app-list reporting components on a rooted Xiaomi 14 running HyperOS 3. The author explicitly credits GPT with the reverse engineering. SystemHelper is one distinct target. Believing it may relate to SIM activation, the author reports installed-app enumeration, usage within the past 24 hours, associated usage/traffic statistics and exclusion of com[.]android-prefixed entries. Payload serialization reportedly includes IMEI, IMSI and ICCID fields. The post identifies a registration endpoint on a China Unicom domain as the reporting destination.

These are author reports about implementation capabilities. No APK revision, hash, code excerpt, GPT revision, invocation conditions, permission checks, packet capture or server response is provided. A field's presence does not establish actual transmission on every invocation, continuous default surveillance on all Xiaomi devices or a causal link to the phone calls. The author did not check reinstallation after removal; claims about extraction/removal without root were not verified here. The separate System Security Component has its own entry rather than conflated functions. Lookup confirms author and full text; no APK was obtained, device accessed, endpoint called or independent reproduction performed.

Shared candidate snapshot: 397 likes, 69,231 views, 27 reposts. Circulation does not validate the findings.
Device is the author's rooted Xiaomi 14/HyperOS 3. Payload capability and actual triggering were not individually verified.

## Sources

- [MeT's GPT/HyperOS 3 two-component analysis report, October 31, 2026](https://x.com/i/status/2116504516317376942)

[中文](../hyperos3-systemhelper-gpt-app-telemetry-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
