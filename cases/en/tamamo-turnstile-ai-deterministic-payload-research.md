# Turnstile payloads: Tamamo reports AI-assisted study of 746 variables and deterministic repeats

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-02
Stage: Needs verification

At 07:22:47 Beijing time on November 2, 2026, Tamamo (@ru_tamamo) reports reverse engineering Cloudflare's bot-detection component Turnstile and building a tool to research 746 variables in its final payload. In contrast with other repositories claiming to reverse it, the author emphasizes a deterministic environment yielding the same payload across runs of obfuscated and deobfuscated code. They say AI reduced the work to about a week versus a task that might previously have taken months.

Original-post lookup confirmed attribution and full text. The 746 variables, determinism and identical payloads are author claims without a tool repository, environment definition, revision, samples or byte-level logs in the post; the attached image was not inspected. Identical payloads do not establish correct semantics for every variable, all-environment coverage, server acceptance or evasion of bot protection. One week is self-reported and months is a counterfactual estimate, not a controlled efficiency comparison. No AI model or REA use is specified. This is a high-level research summary only: no code or Cloudflare test requests were run and no evasion instructions are supplied.

Candidate snapshot: 2 likes, 19 views, 0 reposts. The 746 variables and roughly one week are self-reported; payloads and online effects were not independently checked.

## Sources

- [Tamamo's Turnstile-variable, deterministic-payload and AI-duration report, November 2, 2026](https://x.com/i/status/2117034647645307072)

[中文](../tamamo-turnstile-ai-deterministic-payload-research.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
