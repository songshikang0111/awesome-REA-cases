# SoftProtect: from an abandoned REA self-test to corrections for leaked local source and disabled VM protection

Category: Algorithms and feature recovery · REA
Record date: 2026-11-09
Stage: Analysis test

At 15:51 Beijing time on October 18, 2026, @tokenrebate says SoftProtect gained AI-adversarial measures, tested on a 100-line demo with REA, which reportedly abandoned analysis after half an hour. They also say REA attempted to simulate code from API-call behavior. Earlier retrieval confirmed attribution and wording, not fixture language, protected/unprotected comparisons, countermeasure details, model, tool revision, complete logs or stopping reason. The 100 lines, half hour and abandonment are publisher reports; API-behavior simulation is an attempt, not successful recovery.

At 12:50:55 on November 9, the same @tokenrebate account, now displayed as NullFounder, describes a user demonstration from the preceding day claiming SoftProtect could not stop REA. The first run appeared to reconstruct quickly, but inspection of the AI's reasoning showed it used a Debug compilation path to find local source. That leaks the original implementation through the test environment and is not pure black-box reversing success. Asked to delete the source and repeat, the user still obtained partial recovery; the author then found SoftProtect's VM protection had not been enabled. VM here means the software protector's virtualization feature, not an operating-system VM isolating a test.

The author explains that VM protection has a performance cost and cannot be enabled by default for every user. No overhead numbers or third run with VM enabled are provided. Partial recovery after source deletion is a useful counterexample, but does not establish defeat of every protection configuration or, conversely, that enabling VM works. It is unconfirmed whether these samples are the October 100-line demo; separate self-tests are not presented as a direct regression comparison.

The new post also supplies no program, compiler options, protector revision, AI/REA revision, recovery percentage or logs. Retrieval confirms only the same account, full text and date. No fixture was executed or retested here. Other unreported source remnants, behavioral reconstruction and analysis paths cannot be distinguished. Status remains analysis-test, retaining the author's corrections rather than a universal protection verdict.

October 18 candidate snapshot: 0 likes, 4 views; 100 lines and half an hour are author reports without a public reproducible fixture.
November 9 sealed candidate: 0 likes, 21 views, 0 reposts. The author describes two runs from the preceding day's demonstration, without VM-enabled results or performance measurements.

## Sources

- [TokenRebate's SoftProtect adversarial-fixture self-test, October 18, 2026](https://x.com/i/status/2111726774983995674)
- [Same author's corrections: local source found via Debug paths, a source-deleted rerun and VM disabled, November 9, 2026 at 12:50:55 Beijing time](https://x.com/i/status/2119653939222327509)

[中文](../softprotect-ai-adversarial-rea-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
