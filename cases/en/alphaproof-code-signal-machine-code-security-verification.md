# AlphaProof Code and Signal: a team-reported month to prove key properties of production machine code

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-10
Stage: Related project

A team announcement posted at 20:13:07 Beijing time on November 10, 2026 says Google DeepMind used AlphaProof Code to prove key security properties of production machine code underlying the Signal messaging protocol. The purpose is checking security as the protocol reaches code running on devices, rather than only a simplified design model. It is included as related AI-assisted binary analysis, not traditional decompilation or a Signal clone.

The original post describes AlphaProof Code as an agentic formal-verification framework running on LLMs including Gemini Carbon. It says comparable work could take teams decades of combined effort, while this effort took a month, and announces open formal specifications and verification artifacts. The claim of being the first at this depth for production code of a widely deployed protocol remains attributed to the team; historical priority was not checked here. The post credits Swarat Chaudhuri, Andrew Ferraiuolo, Anton Kovsharov, Tej Chajed, Sam Schlesinger, Karn Seth, Jonathan Katz and Charles Sutton, among others, and thanks Signal for its partnership.

Other candidates relay four weeks, over three million or 6.5 million Lean proof lines, AArch64 and two reintroduced historical bugs. The corresponding specifications, proof repository and verification records were not read, so differing counts are not merged into an established figure. No proof checker was independently run, and the threat model, exact proven components and assumptions were not checked. 'Key properties' does not mean all Signal code, configurations and attack surfaces are free of vulnerabilities. One month is team-reported, not independently measured; REA is not named.

Sealed snapshot: 2,919 likes, 155,181 views, 352 reposts. Engagement is not independent checking of the specification or proof-checker results.

## Sources

- [Candidate: DeepMind team announcement of AlphaProof Code verification of Signal production machine code, November 10, 2026 at 20:13:07 Beijing time](https://x.com/i/status/2120127611137634376)

[中文](../alphaproof-code-signal-machine-code-security-verification.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
