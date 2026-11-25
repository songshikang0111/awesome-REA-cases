# Reconstructing US tax rules in Lean: a report of Lexifina's references and calculation comparisons

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-25
Stage: Needs verification

At 10:55:02 Beijing time on November 25, 2026, Kxians (@xulijian1994), discussing AI and formal verification, relays a project by Alan Yahya's Lexifina team: structure congressional XML for Title 26 of the US Internal Revenue Code, parse statutory references, check existence/validity and generate checkable Lean certificates. This reconstructs executable rules and reference relationships from existing text; it is not decompilation of tax-software binaries. The AI framing comes from the candidate, which does not identify the actual model, division of labor or automation fraction.

The post claims a two-and-a-half-minute check found 138 legislative-text issues, including 67 references to repealed, moved or rewritten provisions, thirty unclosed parentheses and twenty-four spelling/numbering issues, plus duplicate numbers and hierarchical references. It then describes Lean implementations of four parts of 2025 personal income tax: income, deductions, tax computation and credits. Comparisons across 5,000 simulated households and three tax systems reportedly gave 4,993 exact matches with PolicyEngine. That does not establish identical outcomes for the other two systems or legal-authority acceptance of all 138 findings.

Examples in the post include a couple each earning $300,000 obtaining up to $25,000 in state/local tax deductions when filing separately versus $10,000 jointly; a three-child family potentially losing up to $8,046 in earned-income credit when investment income exceeds $11,950 by one dollar; and provisions effective in 2026 affecting 2025 calculations. These remain relayed examples, not tax advice or rules certified here. It further claims that, among sixteen unseen court cases, seventy-nine amounts/rulings with sufficient facts yielded 82% exact agreement and 86% within five dollars, without itemized records or selection criteria.

Retrieval confirms attribution and full text, but the original paper, code, proof certificates, 5,000-household data, three system revisions and sixteen-case list were not read. Passing formal checks validates encoded propositions, not automatically the interpretation, effective year or complete real-world law, and does not replace fact-finding or judges. No experiment date is supplied; November 25 is the post date, not an asserted execution date. REA is unmentioned. Lean was not run and no real tax bill was computed here; status is unverified.

Sealed snapshot: 2 likes, 291 views, 0 reposts, 3 replies. All figures are secondary reports; legal proofs were not reviewed and tax calculations were not performed here.

## Sources

- [Kxians relays Lexifina/Alan Yahya's Lean tax modeling and comparison figures, November 25, 2026 at 10:55:02 Beijing time](https://x.com/i/status/2125422984571826616)

[中文](../lexifina-us-tax-lean-rule-reconstruction-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
