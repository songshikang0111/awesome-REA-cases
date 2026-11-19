# 0sec Labs' 0/0verse: an AI security harness connecting Ghidra, angr and AFL++

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-20
Stage: Related project

At 11:07:13 Beijing time on November 11, 2026, Bobo (@okeyccronald) introduces 0sec Labs' 0 as a security-research control plane over existing models, not a model itself, with local web, headless CLI and MCP. Its reported 0verse binary engine connects Ghidra, angr and AFL++. The account lists fourteen providers or Claude/Codex/Gemini CLI, Apple Silicon macOS, x64/ARM64 Linux and containers, with MIT OR Apache-2.0 licensing. Bobo explicitly has not tested it hands-on; features and licensing remain attributed claims.

At 01:46:27 Beijing time on November 20, 美濃加茂まむ (@superdoccimo) adds a Plan, Discover, Attack, Triage, Verify, Report workflow. Verify reportedly reruns candidates in a separate session, with up to five turns per finding, and proof grades range from candidate to impact-proven. 0verse reportedly exposes nine local MCP tools. Original-post retrieval supplied material omitted at the candidate's ending, but is not implementation auditing or runtime verification here.

The new post lists CVE-2026-68124, a Linux MCTP serial zero-length-frame buffer overflow, CVE-2026-63801, a TIPC asynchronous-decryption use-after-free, and other findings, attributing them to 0sec automated tools. Original CVE records, patches and reproduction logs were not read here. Team-tool attribution cannot be narrowed to the public 0/0verse binary pipeline. Reported XBOW 93/95, black-box union 81/104, cold run 45/104, Cybench 36/40 and npm-audit F1 are self-reported or relayed, not pass@1; they are not generalized into this tool's success rate.

Limits remain research-preview status, default host-shell execution, isolation of untrusted targets and authorized scope. A scope plugin's name does not guarantee sandboxing. Free tooling does not mean free models, and approximately $5.20 per XBOW challenge is not a binary-task cost benchmark. Official code, license text and research pages have not been read here. No dependencies were installed, targets executed or services scanned. REA is unmentioned; status remains related-project.

November 11 sealed candidate: 0 likes, 57 views, 0 reposts. November 20 candidate: 1 like, 233 views, 0 reposts, 0 replies. A source claiming comparison with official material is not this collection's audit or rerun.

## Sources

- [Bobo on 0/0verse, no hands-on testing, safety and cost limits, November 11, 2026](https://x.com/i/status/2120352619826753760)
- [superdoccimo on verification, proof grades and reported results, November 20, 2026](https://x.com/i/status/2123472988192276897)

[中文](../0sec-zero-0verse-ai-binary-security-harness.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
