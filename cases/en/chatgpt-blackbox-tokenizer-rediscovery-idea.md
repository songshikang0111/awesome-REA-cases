# If tokenizer documentation vanished: a ChatGPT-assisted idea for probing token boundaries through a black box

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-15
Stage: Needs verification

At 05:22:06 Beijing time on November 15, 2026, a poster shares a long ChatGPT response to a hypothetical question: if nobody explained tokens, could model behavior reveal discrete internal text units? This is an AI-assisted black-box research design, not a report of recovering a commercial model's tokenizer.

The proposal compares small changes such as cat/cats, spaces and punctuation, then examines API usage counts, costs and context lengths. Further probes cover rare words, affixes, numbers, emoji, camelCase and code fragments. If logprobs or next-token sampling are available, continuation units could provide more evidence. Minimal perturbations and candidate segmentations might approximate a vocabulary and suggest BPE, unigram or related mechanisms. These stages require different observation privileges; ordinary chat output alone does not promise exact implementation recovery.

The full text frames this as a possible discovery path and explicitly allows that the exact tokenizer may not be recovered immediately. No target model/API, test set, counts, segmentation accuracy, vocabulary, code or executed probing is reported. Included as a concrete reversing idea, with ChatGPT assisting the design rather than itself being experimentally characterized. REA is unmentioned. This collection sent no experimental requests and validated no algorithm.

Sealed candidate: 0 likes, 20 views, 0 reposts, 1 reply. Hypothetical research design, without measured results.

## Sources

- [Poster shares ChatGPT's proposal for rediscovering tokens through black-box behavior, November 15, 2026 at 05:22:06 Beijing time](https://x.com/i/status/2121715321749094697)

[中文](../chatgpt-blackbox-tokenizer-rediscovery-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
