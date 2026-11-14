# TinyTurla-NG static reconstruction: compiling C++ and 92.8% structural similarity, not runtime validation

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-10
Stage: Analysis test

At 21:36:11 Beijing time on November 10, 2026, a candidate relays Intezer's AI reconstruction of Slack, Finder and Turla, calling the latter a working replicant. Supplementary reading of Nicole's (@NicoleFishi19) team thread at 23:54 identifies the target more precisely as the TinyTurla-NG backdoor. This entry records defensive static understanding and code reconstruction only, without deployment or attack instructions.

The 23:54:12 post explicitly says the team obtained compiling C++ from static analysis alone, never executed it, and measured 92.8% structural similarity. GPT-5.6 ran the workflow, Kimi K3 reviewed it and Binary Ninja was the stated ground truth. The overview also says the work began with compiled apps and depended on packaging rather than one-click recovery. These later posts support a conservative correction of 'working': compiling code and a structural metric do not establish reproduced backdoor behavior, communications or malicious capabilities.

No sample hash, version, structural-similarity algorithm or denominator, per-function comparison, compilation logs, review records or public code was obtained. The Binary Ninja comparison is project-reported, not independent validation here. The linked article body was unavailable. REA is not named. This collection did not download, compile or execute malware and infers neither provenance, deployment environment nor attack effectiveness.

Sealed candidate: 0 likes, 112 views, 0 reposts. The 92.8% is not byte matching, behavioral equivalence or an attack-success rate.

## Sources

- [Candidate: Intezer research and 'working Turla replicant' account, November 10, 2026 at 21:36:11 Beijing time](https://x.com/i/status/2120148514973819118)
- [Supplementary Nicole team overview identifying TinyTurla-NG, 23:54:10 that day](https://x.com/i/status/2120183240434872570)
- [Supplementary Nicole: static analysis, compiling C++, 92.8% and never-executed boundary, 23:54:12 that day](https://x.com/i/status/2120183247724273962)

[中文](../intezer-tinyturla-ng-static-cpp-reconstruction.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
