# A multistage Windows downloader workshop: Claude Code analysis checked against LimaCharlie telemetry

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-22
Stage: Analysis test

At 12:57:02 Beijing time on November 22, 2026, malware-textbook author Takashi Yoshikawa (@MalwareBibleJP) describes a free two-hour workshop from LimaCharlie. Its concrete target is a multistage Windows downloader. The learning objective is to turn AI-assisted static-analysis predictions into testable detection and response rules rather than simply accept the model's explanation.

According to the post, participants use Claude Code and LCRE for initial triage, capability and indicator extraction and enrichment with external tools, optionally decompiling with Ghidra. They map the analysis to MITRE ATT&CK, design staged responses such as alerting, stopping and isolation, then execute the sample in an isolated Windows VM with LimaCharlie EDR, compare actual telemetry and tune false positives. Recognizing where analyst judgment is needed is another learning goal. The post describes browser-based, per-participant Linux and Windows environments, with Claude remotely controlling Windows so participants do not directly handle the sample. Exercise VMs are said to be free, but participants need their own Claude subscription, a free LimaCharlie account and basic command-line knowledge; prior reverse-engineering experience is not required.

Original-post retrieval confirms attribution and text, but the original course, sample identifiers, model answers, rules and execution logs were not obtained. Two hours is the advertised course length, not measured time to complete reversing. Free access, isolation design and validation workflow are Yoshikawa's secondary course description, not proof all participants get identical results or the environment is absolutely safe. This collection registered for nothing, downloaded or executed no malware, opened no VM and installed no dependencies. REA is unmentioned. Retained as an analysis-test teaching experiment, not an independently reproduced workflow.

November 22 sealed candidate: 4 likes, 521 views, 3 reposts, 0 replies. Live like counts can change and do not replace the sealed snapshot.

## Sources

- [Takashi Yoshikawa describes the Claude Code/LimaCharlie downloader workshop, November 22, 2026 at 12:57:02 Beijing time](https://x.com/i/status/2124366520776347715)

[中文](../limacharlie-claude-code-windows-downloader-workshop.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
