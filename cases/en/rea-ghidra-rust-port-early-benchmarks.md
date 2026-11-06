# REA Rust and a native Ghidra worker: public port documentation fills in an early benchmark lead

Category: Applications and clients · REA
Record date: 2026-11-06
Stage: Related project

At 19:32:18 Beijing time on October 24, 2026, Nicolas Krassas (@Dinosn) shares an early Java-versus-Rust Ghidra-in-REA benchmark headline. At that stage no implementation or figures were obtained. At 09:29:00 on November 6, EveryDev.ai (@EveryDevAi) introduces @linanashi's local Rust port, saying CLI/MCP share handlers, the native Ghidra worker needs no JVM and 195 of 209 frozen tools have native handlers. That is a third-party coverage statement, not 195 semantically equivalent or independently tested tools.

Supplementary lookup finds the matching nanashili/rea-rust and statically reads README at commit 0fb566c88620004af8a4c6f63ccfb56fe7f39962, dated October 26 at 22:53:24 Beijing time, before the candidate. The existing REA/Rust Ghidra investigation ID is retained rather than duplicating the target. This does not establish that the October 24 shortened article points to this repository, nor make the sharers its developers. The project is a Rust port of morluto/rea, with shared CLI/MCP implementations, no Node runtime and a worker in prebuilt releases. Source builds require a separate worker build. Docs describe using the native Ghidra decompiler without a JVM; other analysis providers still require their own installations and Frida is optional. Local tooling does not imply an offline agent or model. README states MIT; license text was not separately read.

README reports an October 24 M1 Pro comparison with warm filesystem caches, frozen builds and seven sessions per version. Go-metadata startup takes 570 versus 64ms, but repeated requests in a running session take 7.3 versus 16.2ms: Rust is not faster on every task. First decompilation of a small C function takes 9.43 versus 0.39 seconds, with sampled peak process-family memory of 1,022 versus 214MiB. The sides use Java and Rust Ghidra respectively, so differences cannot be attributed solely to the implementation language. On a larger Go sample Rust fails from an import-name collision while Java returns all three requested functions. Docs also mention 11 macOS applications plus Go, 125 samples across 25 workflows and failure reruns. Full raw records were not read and the 195/209 count was not audited.

Public documentation now fills the earlier repository/number gap, not proving complete Java Ghidra replacement, cross-platform parity or AI authorship of the port. No build, release installation, target execution or benchmark rerun was performed here.

The older headline remains a shared lead; public implementation docs were read now without establishing a direct match to that old article.
November 6 sealed candidate: 0 likes, 15 views, 0 reposts. The 195/209 count is third-party reporting and performance is project testing; neither was independently executed.

## Sources

- [Nicolas Krassas shares an early Rust/Java Ghidra comparison headline, October 24, 2026](https://x.com/i/status/2113956746242994214)
- [EveryDev.ai's Rust REA introduction and 195/209 handler claim, November 6, 2026 at 09:29 Beijing time](https://x.com/i/status/2118515963494809669)
- [Supplementary pinned README: October 26, 2026 commit, native worker and benchmarks retaining failures](https://github.com/nanashili/rea-rust/blob/0fb566c88620004af8a4c6f63ccfb56fe7f39962/README.md)

[中文](../rea-ghidra-rust-port-early-benchmarks.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
