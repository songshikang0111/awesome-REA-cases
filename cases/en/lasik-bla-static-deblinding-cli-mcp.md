# LASIK: statically removing BLA decoys — 21 million to 17 thousand is an input estimate, not an agent run

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-11
Stage: Analysis test

At 08:00 Beijing time on November 11, 2026, TechVerser (@realfxw) introduces LASIK (LLM Agents Sight In Kode), attributing its deobfuscation passes, boundary tests and MCP server to morphh7 using Claude Code. It aims to help AI read programs hardened against agents by BLA (Blind LLM Agents). This review found public repository pktq/lasik and pinned commit 58f47e047a4d858e29186e5c3dab38ebba8a7786, dated November 10 at 08:20:52 Beijing time, before the candidate window. This is supplementary project material, not a new commit in this window. The post's morphh7 name differs from the repository account; their identity relationship and AI development sessions were not independently established.

Rather than rebuilding a particular commercial app, LASIK removes opaque conditions, unreachable decoys, string encodings with shipped keys, some integrity interlocks, binary padding and model-steering text, so REA and other tools can read a cleaned copy. The README supplies CLI, MCP, library and agent-skill interfaces and says input is never executed. That is not a guarantee of absolute safety for arbitrary hostile files, nor recovery of destroyed names, comments or source. This is a different project from the existing Anti-BLA recovery experiment.

The pinned README and benchmark report estimated input shrinking from 21,104,859 to 16,718 tokens, about 1,262-fold, across 15 files in public BLA CrackMes v6–v9, counting WASM at decompressed size. The documentation explicitly estimates roughly four characters per token for code, two for hex/base64 and one byte per token for binaries. These are not actual agent/REA runs, billed costs, accuracy or cracking-success measurements. A separate experiment hardens one owned small fixture per format with BLA 3.2.1: both default and all-opt-in groups reportedly achieve 21/21 healed, with 11 and 10 files respectively restored byte-identically. Healed does not mean every output is byte-identical, and small fixtures do not establish real large-application coverage.

For BLA 3.2.2, the README lists 59/63 shield files fully healed, with JS/HTML and native coverage still partial. Go, Flutter, Bun, BEAM, APK/DEX and IL2CPP also have limitations involving fixtures generated from BLA source. Static reading of soundness.test.ts finds assertions preserving calls that write through parameters, JSX components, var hoisting, out-of-range integers, aliased mutations, page globals and user integrity checks. These support that the project acknowledges and guards against destructive edits, not a rerun here or external formal proof of arbitrary transformations. The candidate's twelve destructive-edit findings and the README's two independent reviews remain attributed reports, not an independent audit by this collection. No targets were downloaded or executed, dependencies installed or LASIK run. Making a CrackMe readable is not treated as recovering its keys or flags.

Sealed candidate: 0 likes, 5 views, 0 reposts. Original-post retrieval confirms TechVerser attribution; subsequent views do not replace the sealed snapshot.
Pinned commit date: 2026-11-10T00:20:52Z. Documentation and tests are pre-window supplementary evidence, not executed here.

## Sources

- [Candidate: TechVerser on LASIK and Claude Code development, November 11, 2026 at 08:00 Beijing time](https://x.com/i/status/2120305505465979321)
- [Supplementary pinned README: purpose, coverage and limits, commit dated November 10, 2026](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/README.md)
- [Supplementary pinned benchmark: estimates and 21-format owned fixtures](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/docs/benchmark.md)
- [Supplementary pinned regression tests: behavior-changing counterexamples and assertions, read statically only](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/tests/soundness.test.ts)

[中文](../lasik-bla-static-deblinding-cli-mcp.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
