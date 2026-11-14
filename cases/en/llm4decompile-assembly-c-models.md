# LLM4Decompile: C-function recovery and a report on candidate selection and obfuscation training

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-13
Stage: Analysis test

At 00:26 Beijing time on October 22, 2026, @isofunds introduces LLM4Decompile and proposes recovering legacy C/C++ before another model rewrites it for maintenance. That is an earlier collected source; the project README read then is historical research material. The project credits Hanzhuo Tan, Qi Luo, Jing Li and Yuqun Zhang and cites a 2024 paper. The inspected revision is 85b364bf093eb2ee4f3687cfe38a203fca89f23e, committed February 12, 2026.

The README describes Linux x86_64 and GCC O0–O3, first disassembling with Objdump and then generating C. End reads assembly directly; Ref refines Ghidra pseudocode, so input conditions differ. Project evaluation measures execution passing predefined tests and lists 164 standard-library C functions in HumanEval-Decompile and 2,621 real-project functions in ExeBench. Its model table reports 27.3% for 1.3B-v1.5, 46.0% for 1.3B-v2 and 64.9% for 9B-v2; the September 23, 2024 update separately gives 0.6494 for 9B. These are neither arbitrary whole-application recovery rates nor a roughly two-thirds result for 1.3B. The earlier post dates improvement to 2023–2024 and connects it to REA's lineage; the documentation does not establish causality. Bank/insurance migration and subsequent StarCoder rewriting remain proposed uses without deployment tests. Single-16GB-GPU and below-3GB-model-file claims were not independently checked.

At 13:01:02 on November 13, 2026, Takashi Yoshikawa (@MalwareBibleJP) gives a detailed account of a separate study, described as a November 2 arXiv paper by five University of Luebeck researchers, examining selection among multiple LLM4Decompile C candidates. The new candidate is this account. November 2 is the attributed research date, not a new paper within this window. Original-post retrieval confirms attribution and wording, but the paper, dataset and experimental code were not located and inspected here. All new figures below come from this secondary source, not the original model team's older README.

The account describes Ref-9B-v2 and End-6.7B-v1.5 with GCC O0–O3. Given the correct prefix for next-token prediction, the correct token reportedly appears in the top five 95.6% of the time averaged across four input/data conditions; this is not free-generation accuracy. HumanEval-Decompile pass@100, at least one correct answer among 100 candidates, is reported as 93%. Selecting one by lowest perplexity yields 73.3% pass@1 for the pseudocode-input route, compared with 69.0% as the cited prior best. On ExeBench, selection by the number of execution tests passed reportedly gives 86.3%, against an always-correct oracle ceiling of 86.8%. That selector needs exact input/output pairs and is not an unsupervised performance claim for unknown programs.

The account says ExeBench-Obfuscated contains 362,647 entries using OLLVM control-flow flattening, bogus control flow, instruction substitution, or flattening plus basic-block splitting, with project-level train/evaluation separation. After one additional epoch for Ref-9B-v2, evaluation on 1,000 obfuscated samples reportedly improves lowest-perplexity selection from 58.1% to 77.1% and execution selection from 79.5% to 88.8%. These conditions differ from the older README's model table and are not a universal model upgrade. A Mirai leaked-source string-table XOR decryption/re-encryption function compiled at -O2 reportedly scores CodeBLEU 11.3 for Ghidra, 20.1 before training and 27.0 after. Training more closely recovers the bytewise key expression, while types and structure references still differ. Similarity is neither behavioral validation nor coverage of a complete malware sample.

The new study concerns the generation/selection gap and training for particular obfuscations, not proof of arbitrary binary recovery. No models, target code or malware were executed and no scoring repeated here. Status remains analysis-test, explicitly separating earlier inspected project documentation from the current detailed account of an unchecked paper.

Earlier source update: 2026-10-22T00:26:57+08:00; pinned project documentation is not new research in this window.
November 13 sealed candidate: 2 likes, 565 views, 0 reposts, 0 replies. New experimental figures are from Takashi Yoshikawa's account only; paper and scoring were not independently checked.

## Sources

- [isofunds introduces LLM4Decompile and legacy-code maintenance uses](https://x.com/i/status/2112943735394758689)
- [Pinned LLM4Decompile README: model routes, metrics and historical updates](https://github.com/albertan017/LLM4Decompile/blob/85b364bf093eb2ee4f3687cfe38a203fca89f23e/README.md)
- [Pinned revision date and metadata, February 12, 2026](https://github.com/albertan017/LLM4Decompile/commit/85b364bf093eb2ee4f3687cfe38a203fca89f23e)
- [Takashi Yoshikawa reports candidate selection and ExeBench-Obfuscated, November 13, 2026 at 13:01:02 Beijing time; attributed paper date November 2](https://x.com/i/status/2121106036786663600)

[中文](../llm4decompile-assembly-c-models.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
