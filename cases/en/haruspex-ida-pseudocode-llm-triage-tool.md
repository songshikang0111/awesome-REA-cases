# haruspex v1: IDA function pseudocode for pattern matching and LLM vulnerability triage

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Related project

At 06:37:01 Beijing time on November 17, 2026, Takashi Yoshikawa (@MalwareBibleJP) summarizes Hex-Rays' introduction of v1 releases for three IDA tools. Among them, haruspex uses Rust bindings to headless IDA's idalib to export per-function decompiled pseudocode files. Semgrep or weggli can match these to identify binary vulnerability candidates, followed by closer LLM investigation and human static/dynamic checks. The account says haruspex and augur also export structures, enums and other types and adapt IDA's new display format for downstream analysis tools, with IDA 9.5 support discussed.

Supplementary reading covers Marco Ivaldi/HN Security's author article on Hex-Rays, published November 12, 2026 at 19:52:28 UTC, before this window. It explicitly describes this LLM triage chain and credits Claude with helping write new unit, integration and regression tests. On his MacBook Air M3, he reports 280 AArch64 ELF binaries totaling 14 MB taking 827 seconds with tool v0.9.3/IDA 9.3 versus 744 seconds with v1.2.0/IDA 9.5. Runs began without existing IDBs and include initial analysis. Semgrep 1.183.0 reportedly parses about 99.1% of the new pseudocode lines versus 98.3% previously. This is syntactic parseability, not vulnerability-detection accuracy.

A README pinned at e41b312, committed November 16, 2026 at 09:11:37 UTC, confirms per-function files, global/local type headers and latest-IDA support. Tighter Semgrep/weggli integration remains TODO. Stronger LLM integration and LibAFL automatic confirmation are also future plans; current human confirmation is not fully automated. Timings combine tool and IDA upgrades, not an isolated model speedup. The 39.3-minute versus 124-second result belongs only to augur. The other tools have separate entries. Posts, author article and pinned README were read, not full source or test outputs, and nothing was rerun. Neither IDA nor targets were installed or executed. REA is unmentioned; status remains related-project.

The shared three-tool candidate has 4 likes, 414 views, 1 repost and 0 replies at sealing. This is a common snapshot, not separate tool engagement or vulnerability validation.

## Sources

- [Takashi Yoshikawa relays Hex-Rays' three-tool v1 account, including haruspex pseudocode/type exports, November 17, 2026 at 06:37:01 Beijing time](https://x.com/i/status/2122458950763499685)
- [Pre-window supplement: Marco Ivaldi's author article and combined-version benchmarks, November 12, 2026 at 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [Pre-window supplement: pinned haruspex README, committed November 16, 2026 at 09:11:37 UTC](https://github.com/0xdea/haruspex/blob/e41b312c0249854e894ce140c1103cebe3b23031/README.md)

[中文](../haruspex-ida-pseudocode-llm-triage-tool.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
