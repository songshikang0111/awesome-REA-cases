# SwarmLabRE: pi drives REA, checking multi-agent findings against file bytes before reporting

Category: Applications and clients · REA
Record date: 2026-11-18
Stage: In progress

At 19:40:50 Beijing time on November 18, 2026, Nikolaos Chrysaidos (@virqdroid) explains that SwarmLabRE agents run on the pi coding agent and invoke morluto's REA CLI through his own session layer. Supplementary reading of his same-day thread, from 19:36:53 through 19:40:52, identifies the problem as distinguishing invented claims in AI malware analysis. He describes ELF, PE and APK support, up to six agents sharing a board, checking findings against file bytes, building reports from checked facts and separately labeling agent prose as model text.

The author says samples are parsed on the host without execution, while tools and agents occupy separate network-disabled containers and the model key enters neither. Each run reportedly seals input/output SHA-256 hashes in manifest.json. The swarmlabre replay command rebuilds reports offline, returning 0 for identical bytes and 1 for differences.

Public repository search located virqdroid/swarmlabre, and the full README at pinned commit 02db64afb5dce4060fbc06e36eed30a06e24d80a was read. Its November 15, 2026 at 20:06:04 Beijing commit date precedes the candidate and supplies design/validation context only. The document labels alpha 0.1.0, built and checked on one NVIDIA GB10 running Linux arm64 and Python 3.12.3. Demos, tests and eleven golden cases use scripted mocks, not evidence of real-model quality. It separately reports one six-role Qwen3.8 Flash Next run on a generated benign ELF; other listed tested models are Qwen3.8 27B and CYBER-FROST 3.8. Raw traces were not obtained. The README explicitly says no checks use real malware, other CPU architectures are untested and the tools image currently builds only for arm64.

The README extends checks to both file bytes and the run's tool log, explicitly limiting byte-checked to the presence of bytes at an offset, not correct agent interpretation. Verdict, family and confidence remain model opinions. Byte-identical offline recordings do not imply identical second live model runs. Manifests are unsigned: edited files with recomputed hashes can still agree. Replay therefore proves neither source authenticity, complete malicious-behavior discovery nor isolation safety.

Both thread and README describe MIT licensing. Attribution, wording and documentation were read, not the implementation, full security documentation, samples or test logs. No demo was watched, dependencies installed or target run. Host-parser risk, check coverage and key/model communication paths were not independently tested. Retained as an in-progress tool project, not security certification. Supplementary thread posts and the older commit support this candidate, not additional candidates.

Sealed candidate: 0 likes, 19 views, 0 reposts, 1 reply; not functional or security acceptance.

## Sources

- [Candidate: author on pi/REA and the session layer, November 18, 2026 at 19:40:50 Beijing time](https://x.com/i/status/2123018588999049634)
- [Supplementary thread opening: motivation for SwarmLabRE byte checks, November 18 at 19:36:53 Beijing time](https://x.com/i/status/2123017595649396929)
- [Supplement: file formats, six agents and fact-based reporting, November 18 at 19:40:49 Beijing time](https://x.com/i/status/2123018587019358384)
- [Supplement: host parsing, containers and key boundaries, November 18 at 19:40:50 Beijing time](https://x.com/i/status/2123018592031797314)
- [Supplement: SHA-256 sealing and offline replay, November 18 at 19:40:51 Beijing time](https://x.com/i/status/2123018595341123660)
- [Supplementary older README: alpha, mocks and safety/replay limits; commit dated November 15 at 20:06:04 Beijing time](https://github.com/virqdroid/swarmlabre/blob/02db64afb5dce4060fbc06e36eed30a06e24d80a/README.md)

[中文](../swarmlabre-pi-rea-byte-checked-multi-agent-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
