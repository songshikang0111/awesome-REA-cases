# A DSH security and reversing preset: CyHawk flags assumed authorization; later docs add scope gates

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-20
Stage: Related project

At 19:27:09 Beijing time on November 20, 2026, CyHawk Africa (@CyhawkAfrica) describes its review of suixin406/dhs-spenetration, a security-testing and reverse-engineering agent preset for DeepSeek Harness. It reports 56 skills, 49 knowledge materials, CLI utilities and automated decisions, and questions instructions treating supplied IPs, domains or URLs as authorization. This is tooling and safety-boundary research, not a successful intrusion verified by this collection.

Supplementary reading of the most recent pre-candidate commit, 3bfd9e6290c47797e1b3eb25ff732b5f29101029, dated November 20 at 17:12:45 Beijing time, confirms its README and PROMPT. The old prompt explicitly treats supplied targets as authorized without further inquiry. The README heading says 48 substantive articles while its knowledge section says 49 materials; these are not silently treated as one body-text count. The 56 skills and six CLIs are also project claims. Direct reversing features include static/dynamic analysis and protocol reconstruction skills, frontend-bundle API extraction, APK string extraction and cryptography/signature research. None were run here.

At the supplementary 19:54:10 commit c4f4ca5da1c9075090b239b8f04e9cd430e2203a, the README and PROMPT instead declare 74 skills, 48 substantive articles and six CLIs. They require AUTHORIZED-TARGETS.json matching host, port, action, time and authorization reference, default denial and fresh confirmation for destructive actions. This post-candidate revision is evidence of a version change, not a claim already made by the candidate. CyHawk is not credited with causing the change.

The older text supports the review's concern. New gate designs do not prove enforcement on every agent path or production safety. The complete code was not audited, unit tests or dependencies were not run, no targets were probed and skill coverage/counts were not independently verified. This records documentation and revision differences without distributing attack procedures. REA is unmentioned; status is related-project.

Sealed candidate: 0 likes, 27 views, 1 repost, 0 replies. The 56/74 skills and 48 articles/49 materials reflect different versions and definitions, not an independent inventory.

## Sources

- [CyHawk Africa on the DSH preset and authorization concern, November 20, 2026 at 19:27:09 Beijing time](https://x.com/i/status/2123739921210876383)
- [Supplement: README at the pre-candidate 17:12:45 revision](https://github.com/suixin406/dhs-spenetration/blob/3bfd9e6290c47797e1b3eb25ff732b5f29101029/README.md)
- [Same-revision PROMPT: supplied-target authorization assumption](https://github.com/suixin406/dhs-spenetration/blob/3bfd9e6290c47797e1b3eb25ff732b5f29101029/PROMPT.md)
- [Supplement: README at the post-candidate 19:54:10 revision, declaring default-deny gates](https://github.com/suixin406/dhs-spenetration/blob/c4f4ca5da1c9075090b239b8f04e9cd430e2203a/README.md)
- [Same later revision's PROMPT: scope registration and action-gate requirements](https://github.com/suixin406/dhs-spenetration/blob/c4f4ca5da1c9075090b239b8f04e9cd430e2203a/PROMPT.md)

[中文](../dsh-spenetration-reverse-engineering-preset-scope-review.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
