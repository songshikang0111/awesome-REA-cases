# Auditing caramel-1: aniketh uses REA to inspect tensors and source while preserving provenance gaps

Category: Algorithms and feature recovery · REA
Record date: 2026-11-24
Stage: Analysis test

At 02:33:53 Beijing time on November 24, 2026, aniketh (@Aniketh_Deb) explicitly credits REA in a thread-ending reply, recommending hashing artifacts, paging tensors, reading source, auditing the math and separating measurement from inference. Supplementary retrieval of the same thread's 02:33:35–02:33:52 posts supports this candidate only; those posts are not additional candidates. The target is naklecha/caramel-1, a public speech-only conversation model. The researcher says REA streamed 826,411,320 weight bytes, matched the repository's SHA256SUMS and inventoried 137 BF16 tensors totaling 413,198,848 parameters.

He counts sixteen temporal-transformer layers of width 1,024, with 96 tensors and 205,553,664 parameters; six depth-transformer layers of width 512 totaling 154,146,816 parameters; and embeddings, projections, heads and normalization for the remainder. He explains sixteen codec input streams for two speakers, 80 ms steps, codebook delay, CUDA graphs and the lack of explicit VAD/turn-taking rules. A key caveat is that the configuration's source_file_sha256 differs from the day's public source: the configuration names LeanLM/Cfg, whereas code uses Caramel/Config. They may be different snapshots; the configuration fingerprint does not prove identity with current source.

Supplementary reading of the public README, dated November 10, 2026 before this window, finds the model author's description of the two-scale transformer, 11,555 audio hours, 6.2B unique codec tokens, roughly 33B training tokens and approximately two hours fifteen minutes/four GPU-hours of training. It explicitly says most output still makes no sense. The author credits the Cloudy platform with data, model, training and experiments. These are model-project claims, not an independent reconstruction or training-history confirmation by this audit. Only the dynamic README and research thread were read here: weights, full source, a pinned commit, original checksum list and tensor exports were not inspected, and training/inference were not run. No-text training, natural turn-taking and speed cannot be proved by a tensor inventory alone. Figures remain researcher reports, not calculations or reproduction performed by this collection.

Sealed candidate: 0 likes, 12 views, 0 reposts, 0 replies. The 826,411,320 bytes, 137 tensors and 413,198,848 parameters are researcher reports; weights were not audited here.

## Sources

- [Candidate: aniketh credits REA and separates measurement from inference, November 24, 2026 at 02:33:53 Beijing time](https://x.com/i/status/2124934476262474091)
- [Supplementary same-thread target and research introduction, November 24, 2026 at 02:33:35 Beijing time](https://x.com/i/status/2124934403378074087)
- [Supplementary same-thread weight size and reported hash match, November 24, 2026 at 02:33:37 Beijing time](https://x.com/i/status/2124934409375875188)
- [Supplementary same-thread 137-tensor and parameter inventory, November 24, 2026 at 02:33:47 Beijing time](https://x.com/i/status/2124934450702405760)
- [Supplementary same-thread mismatch between configuration and current-source fingerprints, November 24, 2026 at 02:33:52 Beijing time](https://x.com/i/status/2124934472038834348)
- [Supplementary public model README, internally dated November 10, 2026; dynamic version for background only](https://github.com/naklecha/caramel-1/blob/main/README.md)

[中文](../aniketh-caramel1-rea-tensor-source-audit.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
