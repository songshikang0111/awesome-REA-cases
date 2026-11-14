# REA 6.9 on an author's own app: Phosphen reports source-map and Stripe-key exposure plus a release gate

Category: Applications and clients · REA
Record date: 2026-11-12
Stage: Analysis test

At 04:48:26 Beijing time on November 12, 2026, Phosphen (@phosphenq) says they built REA's 6.9 release branch to test new features. The concrete sample is their own test app: the tool reportedly found full source in a source map and a Stripe key the author had left in .env.production. This records the author's client-exposure test, not access to configuration files or credentials by this collection.

The author also describes a one-flag release gate: exit code 3 while high exposure remains, and 0 after fixes. No flag name, exact scan path, key-validity check, redacted output or repair log is supplied. No runnable command is invented, nor is a real production release said to have been blocked. Visible source in a source map does not itself establish disclosure of trade secrets; whether the key worked was not checked.

Retrieval confirms attribution and text. A video is attached but was not reviewed here. The 6.9 version, PR scale, star counts and other format support are promotional context, not independently checked performance or accuracy evidence for this test. The ESP32 test in the same post has a separate case; generic format lists are not split into completed projects. No build revision, sample or full results were reviewed. This collection installed no REA, ran no scan and read no keys.

Sealed November 12, 2026 candidate: 29 likes, 755 views, 0 reposts. This is the whole post's snapshot, not engagement specific to this subtest.

## Sources

- [Phosphen's REA 6.9 own-app and release-gate test, November 12, 2026 at 04:48:26 Beijing time](https://x.com/i/status/2120619685582401814)

[中文](../phosphen-rea69-own-app-exposure-gate-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
