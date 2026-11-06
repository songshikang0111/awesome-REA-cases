# Permuted MNIST: Claude and Codex infer spatial layout from pixel correlations

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-06
Stage: Analysis test

At 08:08:02 Beijing time on November 6, 2026, Robert Lange (@RobertTLange) reports a follow-up to the MNIST WSP weight-programming experiment. MNIST contains 28-by-28 handwritten-digit images. One hidden permutation shuffles the 784 pixels of every image, removing directly visible spatial structure. Claude and Codex are told a permutation exists and may infer it from data. The task is recovering image geometry and constructing classification weights under that condition, not decompiling a commercial model.

The author says correlated inking reveals neighboring pixels and both agents first reconstruct the 28-by-28 layout. Codex uses Isomap plus a lattice fit, reportedly recovering the arrangement after two forward passes; Claude uses partial correlations and simulated annealing. They then resume painting digits into weights. Reported accuracy is 88.8% for Claude versus 88.6% unshuffled, and 87.0% for Codex versus 84.9% unshuffled. The author explains that stored weights look noisy while the first layer's row order encodes the unshuffle. These are figures within one author's setup, not a general comparison of model capabilities.

Original-post retrieval confirms attribution and an attached image, not code, train/test splits, seeds, the definition of the forward-pass budget or repeated-run logs. Two forward passes must not be described as total training cost, nor does this establish recovery of arbitrary unknown permutations. No experiment, image validation or independent accuracy measurement was performed here. REA is not mentioned.

Sealed snapshot: 8 likes, 521 views, 0 reposts. Accuracy, two forward passes and methods are author reports.

## Sources

- [Robert Lange's permuted-MNIST follow-up, November 6, 2026 at 08:08:02 Beijing time](https://x.com/i/status/2118495588979277927)

[中文](../robert-lange-permuted-mnist-agent-spatial-prior.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
