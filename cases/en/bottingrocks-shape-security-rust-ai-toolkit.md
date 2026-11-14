# Shape's JavaScript VM: BottingRocks releases an AI-assisted Rust reverse-engineering toolkit

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-12
Stage: Needs verification

At 12:59:08 Beijing time on November 12, 2026, BottingRocks (@BottingRocks) announces an open-source Shape Security reverse-engineering toolkit targeting Shape's JavaScript virtual machine and its request signals. The author says research began years ago and AI coding agents accelerated a significant part of recent development. Neither a model nor REA is identified; years of research are not attributed entirely to AI.

The author describes a primarily Rust toolkit covering VM bytecode disassembly and analysis, automated JavaScript deobfuscation, execution tracing and program reconstruction, signal extraction and encoding/decoding, SDKs and reproducible examples, plus regression tests across thousands of seeds. The post stresses that understanding the system, reconstructing behavior and validating correctness were central work. These are the author's implementation and testing reports, not tests rerun by this collection.

Supplementary static reading uses the BottingRocks/Shape README at commit ffce7d0cc06333ccdf36614f52abfb741a7c0e5f, committed at 12:50:35 that day before the candidate. It describes parsing captured JavaScript/WebAssembly and tracing a Rust intermediate representation to recover readable programs, with a shared engine for the CLI and Node.js/TypeScript, Python, Go, Rust and C SDKs. Artifacts must match the site, build and session. Runtime-dependent values may stop a trace; readers must check complete/stopped status and unidentified, ambiguous and refused diagnostics. Decoding a field does not guarantee arbitrary edits can be encoded; unsupported edits are refused. This is not described here as a universal cross-site bypass or complete behavior recovery.

Only the README's capabilities and limitations were statically reviewed. The regression corpus, test logs, full implementation and authorization were not audited. This collection downloaded no target scripts, captured no traffic and generated or submitted no signals. Thousands of seeds remains the original post's claim. Public tooling does not establish effectiveness on every production service; status stays unverified.

Sealed candidate: 20 likes, 628 views, 1 repost, 0 replies. Thousands of seeds is the author's reported regression scope, not an independent run by this collection.

## Sources

- [BottingRocks's Shape toolkit release and AI involvement report, November 12, 2026 at 12:59:08 Beijing time](https://x.com/i/status/2120743172813029407)
- [Supplementary pinned Shape README committed November 12, 2026 at 12:50:35 Beijing time, before the candidate; static scope and limitation review](https://github.com/BottingRocks/Shape/blob/ffce7d0cc06333ccdf36614f52abfb741a7c0e5f/README.md)

[中文](../bottingrocks-shape-security-rust-ai-toolkit.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
