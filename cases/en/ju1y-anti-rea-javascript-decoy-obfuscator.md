# Ju1y's anti-rea: local JavaScript renaming and inert decoys, without agent-effectiveness benchmarks

Category: Applications and clients · REA
Record date: 2026-11-02
Stage: Related project

At 02:59:56 Beijing time on November 2, 2026, Ju1y (@Jack_Ju1y) introduces anti-rea, renaming local identifiers and injecting inert decoys into JavaScript bundles during or after builds to disrupt REA and other AI reversing agents. A 02:59:57 follow-up credits veritas's investigation of unusual identifiers disrupting fingerprint-script analysis. This is a defensive related project exploring AI-analysis limits, not a successful AI-assisted reversal of an application.

Supplementary GitHub search found the matching author-name repository JackJuly/anti-rea. README commit 8577c6f886ef667582dca1dba10c3425f767e341 is dated 2026-11-01T18:48:23Z, or November 2 at 02:48:23 Beijing time, before the candidates; shortened-link mapping was not directly verified. Documentation describes local-variable/parameter renaming, unreachable-branch text, single-file/directory/Rollup output support and Vite 6.4.5/Next 16.4.3 App Router client integrations. Next defaults to reporting only; rewriting requires an explicit experimental switch.

Server and identifiable third-party chunks are skipped. Mixed Rollup/Vite chunks receive only inert text; Next skips mixed chunks. Filename filtering cannot reliably detect embedded dependencies. Already named build files do not have content hashes recalculated; source maps can expose original code. Other Vite versions and Next Pages Router are unvalidated, and effectiveness against REA/other agents has not been benchmarked. No source, tests or dependencies were executed/installed here. Retained as an experimental mechanism, not a guarantee of irreversibility, runtime equivalence or security, and distinct from other ANTI-REA repositories.

Main candidate snapshot: 3 likes, 25 views, 0 reposts. Inspiration reply: 0 likes, 5 views.
Actual effectiveness against REA is unbenchmarked. Only static reading occurred; runtime equivalence was not tested.

## Sources

- [Ju1y's anti-rea experimental-project announcement, November 2, 2026](https://x.com/i/status/2116968500334129501)
- [Same-thread attribution of the fingerprint-script research inspiration, November 2, 2026](https://x.com/i/status/2116968502414451121)
- [Supplementary pinned README: integrations and unbenchmarked limits, November 2 at 02:48 Beijing time](https://github.com/JackJuly/anti-rea/blob/8577c6f886ef667582dca1dba10c3425f767e341/README.md)

[中文](../ju1y-anti-rea-javascript-decoy-obfuscator.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
