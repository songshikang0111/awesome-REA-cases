# OGhidra: local or cloud models plan, execute and review Ghidra analysis

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-09
Stage: Related project

At 09:29:41 Beijing time on November 9, 2026, a five-project roundup introduces LLNL's OGhidra, connecting LLMs through Ollama to Ghidra in a plan/execute/review loop for binary analysis, and reports 467 stars. Supplementary reading covered the public llnl/OGhidra README and commit metadata, pinned to 4b91e3f17bc825bc0d41a437cd01fa25e1221d79, committed November 5 at 01:20:19 Beijing time, before this window. This is supplementary project documentation, not a new candidate or independent test. The documentation credits Enoch Wang and is headed OGhidra 3, with a separate orchestrator branch; those implementations are not conflated.

The goal is to reduce repetitive browsing of functions, strings, imports and relationships. Natural-language questions lead the model to call Ghidra tools, review execution results and decide whether to gather evidence or answer. Documented workflows include single-function analysis, bulk naming, security-focused enumeration, semantic search over function summaries, saved sessions and security reports. The MCP backend requires a running Ghidra client, open CodeBrowser and enabled plugin. PyGhidra can run without a GUI; existing projects require a specified program, and direct binary import is also documented. Prerequisites are Python 3.12+, recommended Ghidra 12.0.3 and Java 21 for its extension build. The project lists testing with Ghidra 11.0.3, 11.3.2, 12.0.2 and 12.0.3; these are documentation claims, not a test matrix run here.

Configuration paths cover local Ollama models, external OpenAI/Gemini/Claude APIs and custom compatible endpoints. Only an actually local configuration can support the documentation's privacy aspiration; cloud calls are not data-local guarantees. Over twelve malware patterns, MITRE mappings, automatic naming and reports are project feature claims. No named-target accuracy, false-positive or reconstruction evaluation was obtained; a planning/review loop is not proof of correctness. REA is not used. This collection installed no plugin, ran no model, analyzed no binary and built or executed no target. It is included as a related tool project with inspectable documentation, not successful original-source recovery.

Sealed candidate: 1 like, 21 views, 0 reposts. The post's 467-star snapshot matches supplementary GitHub metadata but does not validate functionality or quality.
The supplementary documentation predates this window; plan/execute/review and listed compatibility versions were not rerun here.

## Sources

- [Current-window roundup: OGhidra's purpose, November 9, 2026 at 09:29:41 Beijing time](https://x.com/i/status/2119603297879458149)
- [Supplementary README at a pinned November 5, 2026 01:20:19 Beijing-time commit, not independent testing](https://github.com/llnl/OGhidra/blob/4b91e3f17bc825bc0d41a437cd01fa25e1221d79/README.md)

[中文](../oghidra-llnl-plan-execute-review-binary-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
