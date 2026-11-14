# REA and gitleaks on owned releases: an author's test reports 73 maps and five false alarms

Category: Applications and clients · REA
Record date: 2026-11-14
Stage: Analysis test

At 18:55:12 Beijing time on November 14, 2026, Archive (@ArchiveExplorer) reports checking their own software the previous night for release exposure. The purpose is to separate secrets in Git history from material users actually receive: gitleaks checks commit history, while REA examines the release directory so scanning source alone does not overlook shipped debugging material.

The author says REA checked five builds and found forgotten source maps in three, totaling 73 .map files, attributed to tsconfig's sourceMap setting. gitleaks reportedly scanned 33 repositories and produced five flags, all judged false positives, including a public contract address and an intentionally planted test key, with zero actual leaks reported. This is the author's triage, not access to keys or scanner-accuracy verification by this collection. A source map can connect shipped scripts to source, but not every map necessarily includes complete source or secrets.

Retrieving the original supplied the full second half: the author proposes Claude explaining each true/false finding, rotating genuine keys first, showing changes for approval before fixing them, and integrating the two checks into commit and release CI. The reported five-build/33-repository results are distinct from that proposed continuing gate; the workflow tree does not establish fully deployed or subsequently clean CI. Node versions, installation commands and exit codes are guidance in that post, not compatibility guarantees checked here.

The author explicitly says neither tool proves an application secure. No target builds, repository inventory, JSON reports, complete fix diff or rerun logs are public in the supplied evidence. Counts, false positives and coverage were not independently checked. This collection read no credentials, ran no scanners, installed no software and changed no target settings. Included as an analysis test with owned targets and concrete reported results, retaining the unverified boundary.

Sealed candidate: 21 likes, 658 views, 2 reposts, 2 replies. Five builds, 33 repositories and 73 maps are author counts, not security coverage.

## Sources

- [Archive's REA/gitleaks owned-release test and proposed Claude workflow, November 14, 2026 at 18:55:12 Beijing time](https://x.com/i/status/2121557557412000032)

[中文](../rea-gitleaks-own-release-exposure-audit-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
