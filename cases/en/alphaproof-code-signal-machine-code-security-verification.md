# AlphaProof Code and Signal: a team-reported month to prove key properties of production machine code

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-11
Stage: Related project

A team announcement at 20:13:07 Beijing time on November 10, 2026 says Google DeepMind used AlphaProof Code to prove key security properties of production machine code underlying Signal. The goal is checking security as the protocol reaches device-executed code rather than only a simplified design model. It is related AI-assisted binary analysis, not traditional decompilation or a Signal clone.

The original post describes an agentic formal-verification framework using LLMs including Gemini Carbon. It says comparable work could take teams decades of combined effort, whereas this took a month, and announces open specifications and verification artifacts. The first-at-this-depth claim for a widely deployed protocol remains team-attributed; historical priority was not checked. It credits Swarat Chaudhuri, Andrew Ferraiuolo, Anton Kovsharov, Tej Chajed, Sam Schlesinger, Karn Seth, Jonathan Katz and Charles Sutton, among others, and thanks Signal for its partnership.

At 15:14:13 on November 11, 青雲 (@echo_vic) relays a reading of the project: libsignal v0.105.4 compiled to AArch64, about 140,000 instructions, five people over four weeks and about 6.5 million Lean proof lines. They describe 40–80 concurrent agents on one machine, 24–72 hours per round, Carbon writing proofs and Carbon with Claude Opus 5.5 drafting specifications for human approval. Two historical bugs were reportedly reintroduced, with machine-checkable proofs that the altered binaries violate theorems, as a check on specification strength. About 26,000 lines of specifications and machine semantics reportedly form the trusted portion. These are an identified reader's detailed claims. Retrieval here confirms their identity and full text only; the original blog, version build, specifications, proof repository and checker records were not read.

Earlier retellings also mention over three million lines; these and 6.5 million are not combined into an established count. Lines, concurrency and four weeks are not accuracy or independently measured labor. The post's comparison with twenty person-years for seL4 crosses targets, specifications and engineering conditions and does not establish a general speedup. Not trusting the compiler does not eliminate the trusted basis: specifications, machine semantics and the proof checker still need scrutiny. No checker was independently run, nor were the threat model, exact components and assumptions checked. Key properties do not mean every Signal component, configuration and attack surface is bug-free. REA is unmentioned.

Older team post: 2,919 likes, 155,181 views, 352 reposts. Engagement is not independent checking of specifications or proofs.
echo_vic's sealed candidate: 0 likes, 18 views, 0 reposts. Version, scale and concurrency are relayed claims; the proof library was not audited.

## Sources

- [DeepMind team announcement of AlphaProof Code verification of Signal production machine code, November 10, 2026 at 20:13:07 Beijing time](https://x.com/i/status/2120127611137634376)
- [echo_vic on the libsignal version, agent runs, Lean specifications and historical-bug counterexamples, November 11, 2026 at 15:14:13 Beijing time](https://x.com/i/status/2120414781471596548)

[中文](../alphaproof-code-signal-machine-code-security-verification.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
