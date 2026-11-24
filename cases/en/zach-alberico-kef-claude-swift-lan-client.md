# A KEF LSX II menu-bar client: Zach credits Claude with a Python-referenced Swift implementation and hardware checks

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-25
Stage: Needs verification

At 00:29:47 Beijing time on November 25, 2026, Zach Alberico (@zalberico) explains that Claude referenced the open-source Python library pykefcontrol rather than capturing KEF Connect traffic. It wrote a native Swift client for the speakers' LAN HTTPS JSON API, including getData/setData, a live event queue and HMAC-signed writes. A supplementary parent post at 00:18:20 the same day identifies KEF LSX II and dissatisfaction with the official iOS app, saying Claude wrote a native macOS menu-bar replacement overnight. That parent is background, not another candidate or evidence of completely reversing the official app.

The author reports reads-first, writes-after tests on his own speaker. Firmware 3.1.141 served only HTTPS on port 4430, with port 80 closed. Frequent new connections caused problems, so the client reuses one connection; power state must come from the active input rather than a potentially stale status field. These are author-reported observations without request logs, public code or other-model tests; sharing code is only an offer. No speaker, HMAC operation or client was tested here. Overnight is the parent's account, not independent timing. This is a different implementation from roberdorfer's USB passthrough/fine-volume bridge, whose latency and sample-rate figures do not transfer. REA is unmentioned.

Sealed candidate: 1 like, 14 views, 0 reposts, 0 replies. Observations concern the author's own device, not independent reproduction.

## Sources

- [Candidate: Zach on Claude, pykefcontrol and firmware differences, November 25, 2026 at 00:29:47 Beijing time](https://x.com/i/status/2125265634783281444)
- [Supplementary parent: LSX II and a macOS menu-bar replacement, November 25, 2026 at 00:18:20 Beijing time; not another candidate](https://x.com/i/status/2125262753078383040)

[中文](../zach-alberico-kef-claude-swift-lan-client.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
