# Metis: static analysis and LLM synthesis for EDK2 boot-protocol fuzzing harnesses

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-04
Stage: Analysis test

At 10:29:21 Beijing time on November 4, 2026, Tanat Tonguthaisri (@gastronomy) relays the abstract of Towards Effective Fuzzing of EDK2 Components. Metis targets TianoCore EDK2 UEFI boot-time interfaces by rehosting protocols as user-space programs. Direct-dependency Component Rehosting (DCR) creates semantically meaningful dependency mocks so both protocol interfaces and dependency interactions become input channels. Static analysis and LLM-guided synthesis generate and refine harnesses, implemented on HBFA.

The abstract reports 60 drivers and 162 protocols, 73.1% coverage, approximately 1.7 times FuzzUEr, and 137 previously unknown bugs. Of 26 reported bugs, 12 are described as remotely triggerable, with all reported items acknowledged by vendors. These are abstract claims: not all 137 bugs are vendor-confirmed vulnerabilities, nor are these this collection's results. Retrieval confirmed the reposter; arXiv lookup timed out. The full paper, revision, samples, coverage definition and vendor notices were not obtained. Model and REA use are unknown. No firmware was downloaded or fuzzer run.

Candidate snapshot: 0 likes, 4 views, 0 reposts. Coverage, bug counts and acknowledgments are attributed to the abstract.

## Sources

- [Tanat relays the Metis/EDK2 paper abstract, November 4, 2026](https://x.com/i/status/2117806376432853251)

[中文](../metis-edk2-llm-guided-rehosting-fuzzing.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
