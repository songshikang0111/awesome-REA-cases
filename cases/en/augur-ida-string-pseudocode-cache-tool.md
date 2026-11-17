# augur v1: string-associated pseudocode and caching, with IDA-version limits on performance claims

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Related project

At 06:37:01 Beijing time on November 17, 2026, Takashi Yoshikawa (@MalwareBibleJP) summarizes Hex-Rays' three-tool v1 introduction. Augur extracts strings and associated function pseudocode, exporting structures, enums and other types like haruspex, for downstream static tools and LLM research followed by human validation. It reuses results to avoid repeatedly decompiling the same function. The account reports 36 AArch64 ELF binaries on the developer's MacBook Air M3 going from 39.3 minutes to 124 seconds.

Supplementary reading covers Marco Ivaldi's Hex-Rays author article published November 12, 2026 at 19:52:28 UTC and augur's README pinned at 9178c4e, committed November 16 at 09:11:12 UTC, both pre-window evidence. The docs confirm upfront decompilation of all functions to recover more strings, then organization of referencing functions and type headers by string; decompilation uses the haruspex API. The article confirms 36 files totaling 2.2 MB, starting without IDBs and including initial analysis, comparing old v0.9.3/IDA 9.3 with v1.2.0/IDA 9.5. The author stresses that timings combine code and IDA upgrades. Binaries with few string references may pay an upfront all-function cost; universally faster operation is not guaranteed.

The article describes deeper LLM triage followed by human static/dynamic confirmation and credits Claude with helping write tests. Tighter LLM integration and LibAFL automatic confirmation remain plans. There was no per-sample verification or independent rerun. Pseudocode candidates are not confirmed flaws, and timings cannot be credited entirely to caching or a model. Haruspex and rhabdomancer have separate entries; performance is not copied to them. Posts, the author article and pinned README were read, not full source or logs. No tool was run. REA is unmentioned; status remains related-project.

The shared three-tool candidate has 4 likes, 414 views, 1 repost and 0 replies at sealing. The 36 files and timings are project-author measurements, relayed by the candidate and checked against the original text, not independently verified.

## Sources

- [Takashi Yoshikawa relays Hex-Rays' three-tool v1 account, including augur caching and the version-limited comparison, November 17, 2026 at 06:37:01 Beijing time](https://x.com/i/status/2122458950763499685)
- [Pre-window supplement: Marco Ivaldi's author article and combined-version 36-file benchmark, November 12, 2026 at 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [Pre-window supplement: pinned augur README, committed November 16, 2026 at 09:11:12 UTC](https://github.com/0xdea/augur/blob/9178c4e9546a80ac2342625fa2049cbd2fcb156b/README.md)

[中文](../augur-ida-string-pseudocode-cache-tool.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
