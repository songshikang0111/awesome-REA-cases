# Qwen3.8-27B-QSA: an account of ryu15 reconstructing sparse attention for long contexts

Category: Algorithms and feature recovery · REA use unconfirmed
Record date: 2026-11-07
Stage: Needs verification

At 11:21:06 Beijing time on November 7, 2026, FHILY (@Oluwaphilemon1) relays Japanese local-inference enthusiast ryu15 reverse-engineering core QSA ideas, expanded in the post as Micro-Block Sparse Attention, and adapting them to Qwen3.8-27B. A checkpoint called Qwen3.8-27B-QSA is said to be on Hugging Face. The goal is reducing long-context attention costs, not recovering the entire Qwen4 architecture; a Qwen4 connection is speculation in the account.

Reported hardware is two NVIDIA V100 32GB GPUs. At 128K context, prefill allegedly rises from about 1,598 to 3,114 tokens/s; at 64K, from about 2,900 to over 4,300. Generation at 128K reportedly rises from just over 20 to over 45 tokens/s. The post describes learned indices for four-token micro-blocks rather than indiscriminately shrinking the KV cache, with most benchmark scores close to the original dense model. These are relayed developer metrics, not measurements here. A model URL, source, original evaluation sets, runtime configuration, precision and itemized quality scores were not obtained; matched conditions and unchanged quality are not established.

This is included as related AI-algorithm reconstruction research, without proof of AI coding-agent assistance or REA use; rea remains unknown. Product naming, the claim that Qwen4 has not launched and architectural attribution were not verified. No weights were downloaded and no model or target code was executed. Status remains unverified.

Sealed candidate: 1 like, 297 views, 0 reposts. Two V100s, token rates and near-baseline quality are relayed claims, not rerun.

## Sources

- [FHILY's account of ryu15's QSA reconstruction and throughput, November 7, 2026 at 11:21:06 Beijing time](https://x.com/i/status/2118906560877371747)

[中文](../ryu15-qwen-qsa-sparse-attention-reconstruction-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
