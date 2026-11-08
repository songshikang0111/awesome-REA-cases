# HyperOS 3 SystemHelper: MeT qualifies earlier GPT findings and reports HTTP encryption details

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-08
Stage: Needs verification

At 20:16:14 Beijing time on October 31, 2026, MeT (@MeTerminator666) says friends received calls demanding removal of X and Telegram, prompting GPT research into app-list reporting on a friend's rooted Xiaomi 14/HyperOS 3. The author thinks SystemHelper may relate to SIM activation and reports app enumeration, 24-hour usage and traffic, exclusion of com[.]android-prefixed packages, and serialization of IMEI, IMSI and ICCID for a China Unicom registration endpoint. Implementation interpretation does not establish transmission every time, continuous surveillance on all phones or causation of the calls. Reinstallation after removal was unexamined; extraction/removal restrictions without root were not checked.

The November 8, 00:40:27 candidate explicitly calls GPT reversing reference-only and requests verification. Retrieval of its 00:03:39 parent finds the author apologizing for hastily publishing implementations without carefully studying activation logic. Claims that SystemHelper records screens, listens or steals private information are described as conflating components; screen-capture implementation belongs to the separately recorded System Security Component. Earlier speculation is not actual surveillance evidence.

The parent adds code interpretation for SystemHelper 3.0.1-20250311 and 3.0.1-20260313: registration defaults to HTTP, with no HTTPS-first fallback. Paths and protocol version, model, manufacturer and sign parameters are visible. POST bodies are AES ciphertext, with the AES key encrypted using an embedded RSA public key and put in sign. No TLS does not mean a capture directly reveals the reported JSON. APK hashes, code excerpts, GPT revision, activation conditions, permission checks, traffic and server responses remain absent for independent validation. The parent supplements rather than replaces the candidate.

Only author and text were confirmed. Images were not viewed, and no APK was obtained, device accessed, endpoint called or reproduction performed. Temporary-root/removal suggestions are not validated fixes.

Older candidate: 397 likes, 69,231 views, 27 reposts. Circulation does not validate conclusions.
Device is the author's rooted Xiaomi 14/HyperOS 3. Capabilities and actual activation were not individually verified.
November 8 sealed candidate: 6 likes, 1,333 views, 0 reposts. HTTP and AES/RSA are the author's static interpretation, not packet-capture validation.

## Sources

- [MeT's GPT/HyperOS 3 two-component analysis report, October 31, 2026](https://x.com/i/status/2116504516317376942)
- [MeT asks readers to verify GPT findings, November 8, 2026 at 00:40:27 Beijing time](https://x.com/i/status/2119107723933663535)
- [Supplementary parent: activation-logic correction, component separation and HTTP/encryption interpretation for two revisions, November 8, 2026 at 00:03:39 Beijing time](https://x.com/i/status/2119098463682166820)

[中文](../hyperos3-systemhelper-gpt-app-telemetry-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
