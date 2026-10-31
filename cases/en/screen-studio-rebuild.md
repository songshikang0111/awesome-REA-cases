# Screen Studio rebuilds: an REA usage report and Dolly's screenshot-driven plan

Category: Applications and clients · REA
Record date: 2026-10-31
Stage: Needs verification

Screen Studio is a desktop screen-recording and presentation tool. The existing October 13 author report says REA dissected the app and Claude Code built a replica from its rules in about half an hour, with the new version recording its own demo. No reconstruction code, feature list or comparison tests were supplied. Functional/visual parity, timing and the recording process remain independently unverified.

At 17:58:54 Beijing time on October 31, 2026, darkzodchi (@zodchiii) reports using Opus 5.5 to rebuild a Screen Studio-style auto-click-zoom recorder for Mac and Windows. Supplementary reading of the complete 19:41:55 prompt in the same thread identifies it as Dolly: infer functionality from screenshots without copying code, names, icons or assets; first design six concepts and a specification, then split work into eight areas covering capture, zoom, cursor, editor, export, captions, licensing and installers. The requested stack is Electron/React/TypeScript, FFmpeg and whisper.cpp, with local captions and GitHub Actions packaging. This is another author's approach to the same target functionality, not proof of identity with the earlier project. REA is not specified for Dolly.

The main post still contains unfilled test and timing placeholders such as [what it found], [what broke] and [time spent]; the prompt retains price and checkout-URL placeholders. Its 'fully free' claim is qualified by an open-core specification: free export is listed as 1080p30, while 4K/60fps, captions and other features are planned as Pro. Acceptance then asks for 1080p60, an unresolved inconsistency. Requested tests, eight-agent review, offline captions, installers and MIT licensing are not implemented facts. No pinned code, CI results or real recording/export were obtained; attachments were not watched. No version was installed or run here. Unverified status remains.

Posted: 2026-10-13T11:06:29+08:00 (Beijing time)
The earlier author reports REA and Claude Code; the new author specifies only Opus and does not inherit REA attribution.
New candidate snapshot: 35 likes, 1,274 views, 4 reposts. The supplementary prompt is not an executed test record; free/Pro and acceptance specifications remain inconsistent.

## Sources

- [Author's original post on REA analysis and reconstruction](https://x.com/i/status/2109843188341207283)
- [Darkzodchi's Dolly/Opus reconstruction report, October 31, 2026](https://x.com/i/status/2116469955042668870)
- [Supplementary complete Dolly prompt and acceptance requirements, October 31, 2026 at 19:41 Beijing time](https://x.com/i/status/2116495881101041955)

[中文](../screen-studio-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
