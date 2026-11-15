# WindowsiOS: Gemini-assisted ARM64 translation and Windows compatibility, with an author-reported Windows 11 iPhone demonstration

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-15
Stage: Needs verification

At 11:52:06 Beijing time on November 15, 2026, Andrew111 (@AndrewSignalZ) relays a claim that Ammaar Reshi used Gemini 4 Carbon to run Windows 11 24H2 on a device called iPhone Duo. The goal is an interactive Windows ARM64 environment inside an iOS app, not Windows source recovery or proof of bare-metal Windows boot on an iPhone. The post mentions a demonstration video, but this collection did not obtain or watch it.

Supplementary research located ammaarreshi/WindowsiOS and read the README pinned at 0071d6975287fd720b9046dfd3bd80b6f2aa765e, committed November 12, 2026 at 03:25:11 UTC, before the window. It supports architecture and attribution only. Documentation credits Gemini 4 Carbon for the bring-up while explicitly building on Henge/Husk ARM64 dynamic translation and software MMU work, LinuxRunner, StikDebug, libslirp, EDK2 and virtio-win, among others. This is not a model completing everything independently from scratch.

Documented compatibility problems include supporting Windows NT's 4 KB pages and process ASIDs on a 16 KB Darwin host, correcting exclusive atomic instructions and Prism unaligned memory accesses, and providing UEFI/ACPI, NVMe, USB, audio and network virtual devices. The project says it avoids Hypervisor.framework and instead uses ARM64-to-ARM64 JIT plus a software MMU. Its 'near-native' wording therefore does not mean no emulation, no virtual hardware or measured original-device speed. Prism provides x86/x64 compatibility inside the guest, not proof that every Windows application works.

The README claims end-to-end verification on iPhone19,4/A20 Pro/iOS 27 TXM, with showcase descriptions covering Edge, Antigravity 2.31.0, audio, Ethernet and an OAuth bridge. It also reports a 384 MiB JIT, 4.5 GB guest RAM and 1.46 GB idle desktop memory. These remain project claims: screenshot authenticity, test logs, device identity and performance data were not checked. The candidate's approximately 12 GB image was also not verified. Detailed documentation is not independent validation.

Build instructions require an Apple Silicon Mac and developer tools, a legally obtained Windows ARM64 image and separately supplied firmware/drivers, with LLDB assisting JIT. None of those commands was run here. The README states GPL-2.0-or-later for the code, excludes Windows images from distribution and lists upstream licenses. Full licensing was not reviewed, and Windows or device restrictions are not deemed authorized. Retained as an unverified AI-assisted system-behavior adaptation and binary-translation project. REA is unmentioned. This collection downloaded no OS image, installed no dependencies, compiled nothing, connected no phone and performed no reproduction.

Sealed candidate: 1 like, 33 views, 0 reposts, 0 replies. No independent performance or stability test.
Windows 11 24H2, Gemini 4 Carbon, iPhone Duo and memory figures are attributed as supplied by the sources; promotional 'native' wording is not treated as bare-metal execution.

## Sources

- [Andrew111 relays a WindowsiOS/Gemini Windows 11 phone demonstration, November 15, 2026 at 11:52:06 Beijing time](https://x.com/i/status/2121813465946022308)
- [Pre-window pinned WindowsiOS README: Gemini attribution, upstreams, JIT/MMU architecture and project-reported validation, committed November 12, 2026 at 03:25:11 UTC](https://github.com/ammaarreshi/WindowsiOS/blob/0071d6975287fd720b9046dfd3bd80b6f2aa765e/README.md)

[中文](../windowsios-gemini-arm64-windows-iphone-compatibility-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
