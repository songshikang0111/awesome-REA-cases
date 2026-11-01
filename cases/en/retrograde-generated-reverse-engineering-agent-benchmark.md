# RETROGRADE: generated programs and behavioral execution for evaluating reverse-engineering agents, with Round 0 pending

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-01
Stage: In progress

At 09:15:28 Beijing time on November 1, 2026, celeste (@vmfunc) introduces RETROGRADE to address static hand-built reverse-engineering benchmarks leaking into training data and flag/text-similarity scoring rewarding recognition rather than understanding. The author says targets are generated only after seeds are drawn, with programs and ground truth constructed from one intermediate representation, and claims graded by behavioral execution.

Supplementary author posts at 09:15:29–09:15:31 describe 15 workloads, C/C++/Rust/Go and six ISAs, including CRC/state-machine wire protocols, randomized bytecode VMs, license checks, CAN/UDS automotive ECUs, BLDC control, DSP and a benign malware-behavior surrogate. A ten-pass protection lattice includes mixed Boolean arithmetic, opaque predicates, flattening, string encryption, anti-debugging, virtualization, packing and off-ABI conventions. The author claims per-instance behavior-preservation checks to isolate protection effects; this collection did not validate all generators.

One example has 0.9999 text similarity but scores 0.048 after flipping a comparator. Claims require confidence and an evidentiary address; equal-accuracy overconfident/calibrated examples score −0.76/−0.05. These illustrate the method, not a model's full-benchmark result. The thread publishes a Round 0 seed commitment hash and promises the key with results, saying a CC BY 4.0 methods paper is available and results/full transcripts will follow. The paper, repository and actual Round 0 results were not obtained. Proven resistance to leakage or testing of REA cannot be inferred. No generator, target program or evaluation was executed here.

Candidate snapshot: 38 likes, 1,793 views, 4 reposts; changing lookup counts do not replace it.
Supplementary thread posts are the author's November 1 methodology descriptions. Paper not read, evaluation not run and Round 0 model results not obtained.

## Sources

- [celeste's RETROGRADE announcement, November 1, 2026](https://x.com/i/status/2116700618660470792)
- [Supplementary thread: IR generation, 15 workloads, four languages and six ISAs](https://x.com/i/status/2116700620682125360)
- [Supplementary thread: execution scoring and flipped-comparator example](https://x.com/i/status/2116700622313656727)
- [Supplementary thread: confidence and evidentiary-address scoring](https://x.com/i/status/2116700623949504966)
- [Supplementary thread: concrete workloads and architectures](https://x.com/i/status/2116700625744601237)
- [Supplementary thread: ten-pass protection and behavior-preservation claim](https://x.com/i/status/2116700627187450256)
- [Supplementary thread: Round 0 seed commitment](https://x.com/i/status/2116700628676435998)
- [Supplementary thread: methods paper and forthcoming results](https://x.com/i/status/2116700630006030475)

[中文](../retrograde-generated-reverse-engineering-agent-benchmark.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
