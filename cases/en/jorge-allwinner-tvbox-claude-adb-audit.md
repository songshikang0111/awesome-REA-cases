# Allwinner TV box: Jorge reports Claude/ADB findings at the system layer

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-10-31
Stage: Needs verification

At 21:49:04 Beijing time on October 31, 2026, Jorge Pozo (@pozojorge) reports asking Claude to analyze his generic Allwinner TV box through ADB. It had Xuper and two other apps. Beyond excessive app permissions, he reports firmware impersonating a Google device, passwordless ADB enabled by default, disabled SELinux, factory root and a 2025 image carrying a 2022 security patch. He claims an undeletable hidden system installer had silently installed four apps disguised with Android-system names, requesting camera, microphone, location and Google-account permissions.

The box reportedly maintained connections to unusual ports on Chinese servers while idle. Combining this with an earlier ISP unusual-traffic warning and slow internet, he infers third-party traffic relaying; that is not captured proxy content or attribution proof. He believes factory reset cannot clean the relevant partition, says guest-network checks found no access to his phones or computer, and permanently disconnects power. No raw logs, model, firmware hash, package names, traffic records or reproducible steps substantiate these conclusions. They establish neither universal model risk, absence of lateral access, impossibility of repair nor safe eradication.

Full original-post lookup confirms the author and the closing isolation/disconnection account; the long source was read through its end. No Claude revision or REA use is identified. No box was connected, ADB run, server accessed or independent reproduction performed here. Retained as a defensive AI-assisted device-analysis report.

Candidate: 12 likes, 849 views, 2 reposts. Four apps and the 2022/2025 dates are author reports.

## Sources

- [Jorge's complete Claude/ADB TV-box analysis report, October 31, 2026](https://x.com/i/status/2116527880473649153)

[中文](../jorge-allwinner-tvbox-claude-adb-audit.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
