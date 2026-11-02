# ClipShare: vartekx's Opus-built LAN clipboard alternative for Mac, Windows and iPhone

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-02
Stage: In progress

At 07:12:49 Beijing time on November 2, 2026, vartekx (@vartekxx) presents ClipShare as reverse engineering Apple's clipboard with Opus 5.5. The goal is copying on Mac and pasting on Windows, with iPhone joining through a web page instead of messaging oneself. Starting in an empty directory with 'AirDrop, but between PC and iPhone', Claude Code reportedly chose a Python-standard-library local service. Because iOS restricts background clipboard access, two signed Back Tap Shortcuts replace that path.

The author reports 40 end-to-end tests and a byte-for-byte 40MB file round trip. They describe fixing failed macOS global-broadcast discovery, an onboarding loop requiring an address to be pasted before clipboards were connected, and two running instances showing different pairing codes. Automatic discovery, a six-digit pairing code and duplicate-start prevention reportedly resolve these. One evening, zero personally written code, 62KB and two final files are author claims, alongside a Vercel landing page and Remotion promo, not this collection's timings, source counts or hardware tests.

The same author's full build prompt at 07:12:50 was read as supplementary thread material, not another candidate. It requests Windows Win32 calls through ctypes, Mac pbcopy/pbpaste, bidirectional connect mode in the same file and iPhone Safari access. Streaming files up to 2GB, a request secret, a fresh code on restart, a one-minute lockout after five wrong attempts, OS-marked private-clipboard filtering and memory-only history are requirements, not audited implementations. It explicitly warns that LAN traffic is plain HTTP for home Wi-Fi. No cloud does not mean encryption or established security; a 40MB self-test does not verify the 2GB limit.

Only the original post and author thread were read. Repository short links were not resolved, source/demo not inspected and the service not run. No real clipboard, key or pairing was accessed. The described ordinary OS interfaces support a functional alternative, not demonstrated recovery of Apple's Universal Clipboard/AirDrop private protocol or guaranteed automatic background synchronization on every system.

Candidate snapshot: 12 likes, 324 views, 0 reposts. Forty tests, 40MB, one evening, 62KB and two files are author reports.
The 2GB limit, secrets, private-marker filtering and lockout are prompt requirements, not source/security verification. LAN traffic is plain HTTP.

## Sources

- [Candidate: vartekx's ClipShare build, test and pairing-debugging report, November 2, 2026](https://x.com/i/status/2117032140009594890)
- [Supplementary author thread: full build prompt and plain-HTTP limit, November 2 at 07:12:50](https://x.com/i/status/2117032145139204569)

[中文](../clipshare-vartekx-opus-cross-platform-lan-clipboard.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
