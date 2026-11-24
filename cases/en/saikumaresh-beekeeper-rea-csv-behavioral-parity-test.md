# Beekeeper Studio CSV export: REA's clone reportedly matches 90 cases, but upstream specifications still have gaps

Category: Applications and clients · REA
Record date: 2026-11-24
Stage: Analysis test

At 14:07:30 Beijing time on November 24, 2026, Sai Kumaresh (@saikumaresh_ai) reports testing Reverse Engineer Anything against one feature: CSV export in the open-source database client Beekeeper Studio. Supplementary author posts from 14:07:45 to 14:09:18 describe an analyst seeing only the packaged app, a builder seeing only the analyst's specification, a grader checking the specification against real source and a fourth agent comparing original and clone. Clean room describes the author's information separation, not a legal clean-room certification or a complete contamination audit by this collection. Models and exact software versions are not disclosed.

The author reports whole-app analysis timing out and then exhausting memory after 35.7 minutes, versus six seconds for a roughly 70 KB slice of one feature. Different input scopes do not establish an equal-task speedup or total project duration. Reported comparisons match all 18 edge cases byte for byte and 90/90 across five database dialects. The clone reportedly also preserves large-ID precision loss, identical exports for NULL and empty string, and formula strings written unchanged. These are the author's behavioral comparisons, not tests rerun here or proof for all inputs.

The author still declines sign-off: the file-writing specification scores 95.5%, but upstream gaps include visible-column selection, a 50,000-row grid cap, column types sourced from different paths and filters not passed through. Identical final files under frozen inputs establish only the last writing step, not equivalent data selection in the real UI or the complete export workflow. The short thread does not detail the 95.5% scoring definition, coverage or dialect environments.

A separate candidate at 14:09:18 in the same thread links a full article, all logs and a parity harness. That post is retained as an entry point; its short links were not expanded or their contents obtained here. No harness was read, test run, complete isolation record audited or result reproduced. Only the author thread was read; status remains analysis-test.

The two sealed candidates respectively have 0 likes/11 views/0 reposts/2 replies and 0 likes/10 views/0 reposts/0 replies. All test counts, durations and scores are author reports, not independently rerun.

## Sources

- [Sai Kumaresh introduces the four-agent REA experiment, November 24, 2026 at 14:07:30 Beijing time](https://x.com/i/status/2125109033686421547)
- [Supplementary author thread: Beekeeper CSV target and four-role separation, 14:07:45](https://x.com/i/status/2125109096642998506)
- [Supplementary author thread: whole-app failure and 70 KB slice, 14:08:01](https://x.com/i/status/2125109163827364185)
- [Supplementary author thread: 18 and 90 comparison results, 14:08:15](https://x.com/i/status/2125109222472101909)
- [Supplementary author thread: precision, nulls and formula strings, 14:08:32](https://x.com/i/status/2125109293699785113)
- [Supplementary author thread: 95.5% score and upstream gaps, 14:08:47](https://x.com/i/status/2125109356614361240)
- [Supplementary author thread: limits of final-file parity, 14:09:03](https://x.com/i/status/2125109423807070660)
- [Separate candidate linking the article, logs and harness, November 24, 2026 at 14:09:18; linked contents not read](https://x.com/i/status/2125109486767714438)

[中文](../saikumaresh-beekeeper-rea-csv-behavioral-parity-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
