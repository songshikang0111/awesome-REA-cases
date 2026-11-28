# Static review of a purported 224GB GTA VI build: rootcmoi acknowledges AI amid coverage criticism

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-28
Stage: Analysis test

At 06:59:25 Beijing time on November 28, 2026, @dddisasteroIogy quotes rootcmoi's investigation, mocking 'Ghidra plus finished screening 224GB' as merely asking Claude. Another candidate at 07:42:04 recommends IDA and warns against trusting all Claude output, especially treating 224GB of binaries as completely analyzed. These are criticism and advice, not new measurements or proof that the author used IDA or Claude actually read all files.

Supplementary reading identifies the target through the original post at 03:49:01, before this window. @rootcmoi reports a read-only review of 224GB across 109 files in a purported GTA VI Xbox build, without executing binaries. Findings include a roughly 120MB main EXE with Flash/ActionScript 3 and apparent Scaleform traces; an EXE-looking .bin that is actually an Xbox catalog without executable code; and a DLL using CreateRemoteThreadEx only to create a thread in its own process. Twelve Microsoft DLLs reportedly have Authenticode digests inconsistent with embedded signatures, with origins unresolved. An EXE timestamp of November 13, 2026 at 22:40 is an embedded value, not a build publication date confirmed here. The author reports no malware, infostealer or C2 identified within the analyzed scope while explicitly denying any safety guarantee.

In a reply at 07:15:29 within this window, the author says PE parsing and integrity checks were automated, particular issues were investigated in Ghidra, and AI was used. That reply does not name a model; Claude attribution comes from critics, not a verified tool transcript. The supplementary original supplies target and findings context rather than another window candidate. File hashes, complete scripts, disassembly records and checkable samples are absent. Build authenticity, signature-mismatch causes and safety remain unestablished. No suspected leaked game files were obtained, distributed or run here; static non-detection is not certification. REA is unmentioned.

06:59 candidate snapshot: 0 likes, 31 views, 0 reposts, 2 replies. 07:42 candidate: 0 likes, 6 views, 0 reposts, 0 replies. Engagement with criticism does not validate findings.

## Sources

- [Window candidate criticizing Claude/Ghidra and 224GB screening, November 28, 2026 at 06:59:25 Beijing time](https://x.com/i/status/2126450851577257989)
- [Window candidate recommending IDA and questioning exhaustive Claude analysis, November 28, 2026 at 07:42:04 Beijing time](https://x.com/i/status/2126461584776347732)
- [Supplementary original: static-review scope and findings, November 28, 2026 at 03:49:01 Beijing time, before the strict window](https://x.com/i/status/2126402936490139648)
- [Supplementary author reply: PE parsing, integrity checks, Ghidra and AI, November 28, 2026 at 07:15:29 Beijing time](https://x.com/i/status/2126454896484327877)

[中文](../rootcmoi-alleged-gta6-build-ai-ghidra-static-review.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
