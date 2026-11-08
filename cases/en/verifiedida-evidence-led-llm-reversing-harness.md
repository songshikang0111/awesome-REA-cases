# VerifiedIDA: evidence, edit receipts and resumable model-led IDA investigations

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-07
Stage: Related project

At 23:47:26 Beijing time on November 4, 2026, Ryan Naraine introduces SentinelLabs' VerifiedIDA as inspectable, continuable and reusable LLM reversing. SentinelOne's official account confirms the project and evidence focus at 23:57:10. Supplementary lookup found SentineLabs/verified-ida. README, usage, worked-example and SECURITY were read at caab127be22a071d93a9b4737ff65c39b57842c8, committed September 15, 2026 at 01:19:07 Beijing time, before this window. November publicity is not treated as a new source release.

The project addresses findings stranded in chats, annotations overstating code behavior and success claims lacking checkable results. A model chooses investigations and proposes names, comments, interfaces and shared types. The host checks targets and current evidence, applies edits to a candidate IDB, checks results, records a ledger and receipts, and accepts changes into the working database. A notebook preserves progress and questions. Independent review is a separate command, not automatic in analyze. Optional coverage reconciliation is disabled by default and does not require annotation of every function.

The project's ComRAT example is a recorded static investigation without executing malware. Sol uses a 48-byte offset in a CreateProcessW argument to infer a structure. Saving SuspendedProcessContext produces a measured use count of zero; changing a function parameter to its pointer produces one and decompilation shows ctx->process_info. A fresh IDA process reopens the saved database and the receipt reports verified. The unknown_28 field remains unexplained. This supports the illustrated edit and persistence checks, not correctness of all structure semantics or malware conclusions. Reviewers can also miss errors. This collection did not rerun the trace.

The supported environment is Linux, Python 3.10+, IDA Pro 9.3 and Hex-Rays, with a user-supplied license and model access. MIT source is not free IDA. Documentation describes network-disabled IDA workers and scripts using disposable databases, without launching samples as programs. The controller still sends code, results and context to a model provider, and IDBs contain sample bytes: this is not purely offline or inherently safe. Independent review defaults to 250M recorded tokens, 2,500 requests and four active hours, not this example's measured bill; cached tokens count and response-boundary checks may cross a ceiling. No dependencies, IDA or samples were installed or run here.

A new Japanese retelling at 16:11:01 Beijing time on November 7, 2026 adds an experimental call-flow mode: before finalizing a function's conclusion, the model must investigate every direct internal callee. On one ComRAT function, the model reportedly examined 20 direct callees without being told which mattered, identifying recursive forwarded-export resolution missed in six previous attempts. Initial global application generated 265 mandatory investigation nodes for eight edits, prompting narrower scope. The account says evaluation mainly used GPT-5.6 Sol and exposed inaccurate naming, findings absent from IDBs, lost plans and prematurely stopped investigations. The new article and code revision were not read here. These figures are not assigned to the earlier pinned commit as verified behavior, and persistence checks are not semantic validation.

Sealed candidates: Ryan, 1 like, 142 views, 0 reposts; SentinelOne, 0 likes, 97 views, 0 reposts. Later engagement does not replace these snapshots. Verified means database-edit verification, not a certificate of semantic correctness.
November 7 sealed candidate: 9 likes, 649 views, 1 repost. Twenty callees, six missed attempts and eight edits/265 nodes are new secondary reporting, not independent retesting.

## Sources

- [Ryan Naraine introduces VerifiedIDA, November 4, 2026 at 23:47:26 Beijing time](https://x.com/i/status/2118007217647726704)
- [SentinelOne's official project introduction, November 4, 2026 at 23:57:10 Beijing time](https://x.com/i/status/2118009669239153074)
- [Supplementary pinned README; commit predates this window](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/README.md)
- [Static ComRAT type-application example at the same commit](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/docs/worked-example.md)
- [Usage, review and budget limits at the same commit](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/docs/usage.md)
- [Isolation and model-provider data handling at the same commit](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/SECURITY.md)
- [Japanese account of ComRAT call-flow investigation and scope expansion, November 7, 2026 at 16:11:01 Beijing time](https://x.com/i/status/2118979524046278875)

[中文](../verifiedida-evidence-led-llm-reversing-harness.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
