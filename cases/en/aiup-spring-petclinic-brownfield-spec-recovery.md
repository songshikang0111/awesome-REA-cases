# AIUP's PetClinic example: recover use-case specifications from existing code, then maintain incrementally

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-05
Stage: Related project

At 02:35:56 Beijing time on November 5, 2026, Simon Martinelli (@simas_ch) introduces a brownfield section for AI Unified Process, or AIUP. For systems whose code predates specifications and whose authors may have left, it recovers use-case diagrams, use-case specifications and an entity model from existing code. Requirements Engineer and Software Engineer review errors and open questions together. A spec review accepts current findings as a baseline so only new issues fail the build, and records the existing stack without demanding framework migration.

The maintenance path reconciles specifications with code on the existing stack rather than regenerating everything. The modernization path uses the old system as requirements input, migrating one use case and module at a time. The concrete showcase is Spring PetClinic: the author says start is after reverse engineering and main has all use cases implemented and tested. He explicitly calls it tiny; a larger example is only planned.

A confirmed repository, branch diff, specifications, test logs, model and agent execution records were not obtained. Starting without existing tests is a process claim. Tests generated from recovered specifications do not independently establish equivalence with original behavior, and failures need not be product defects. Included as AI-related code-to-specification recovery, not binary decompilation or demonstrated large-system migration. No code was run; REA is not mentioned.

Sealed snapshot: 4 likes, 245 views, 3 reposts. The start/main states are author statements; branches were not checked.

## Sources

- [Simon Martinelli's AIUP brownfield workflow and PetClinic showcase, November 5, 2026](https://x.com/i/status/2118049623906648130)

[中文](../aiup-spring-petclinic-brownfield-spec-recovery.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
