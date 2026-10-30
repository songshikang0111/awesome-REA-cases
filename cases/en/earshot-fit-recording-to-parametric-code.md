# Earshot fit: reconstructing a reference recording as adjustable code

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-10-30
Stage: Analysis test

At 22:25:58 Beijing time on October 30, 2026, 小能猫 (@n7wb1l) presents Earshot for CPU-local audio description, matching, critique and MCP integration with agents such as Claude Code. Its fit command translates recordings into adjustable Forge Recipes. Public search found the corresponding Leonxlnx/earshot description; its README was read at commit 591fa3e028032e6dce56620a20e932e35667e8d8, dated 2026-10-22T10:07:51Z. This predates the candidate and is supplementary, not a confirmed short-link destination.

Using analysis by synthesis, fit estimates ringing modes, tracked partials, time-varying noise or hybrid models, then outputs a Python recipe with render(). Size, damping, pitch, brightness and decay can be changed, and two recordings morphed. The target is an editable generative structure behind a reference sound, not recovered recording-software or model internals. The project describes CPU-local operation; optional Gemini audio critique requires explicit upload consent and the user's key, so not every path is network-free.

The README labels a median CLAP cosine of 0.945 on 12 recordings, matching tags in 10/12, and a one-listener 12-trial blind test as earlier 0.2–0.3 engine results, explicitly not rerun on 0.4. Version 0.4 was tuned on 78 development clips. On 38 opened held-out clips its median is 0.903 versus 0.878 for 0.3. On a harder fresh 28-clip set the median is instead 0.851 versus 0.853, mean 0.860 versus 0.844, and mel gap 0.58dB versus 0.87dB; passing variations fall to seven from eight and onset error rises to 1.00 octave from 0.53. Selective improvements do not establish universal superiority or indistinguishability.

Reference audio is privately licensed and not distributed. Similarity and mel metrics are proxies, and 0.4 had no human listening test. Documentation acknowledges that optimization can fool its realness model and calls for model-free measurements and blind listening. Recipes are derivatives of the recording and should retain its license. The candidate's roughly 3.1k stars were not independently checked. This collection only read documentation, without installing, fitting audio, executing generated code or rerunning tests. Analysis-test status is not independent reproduction.

Candidate snapshot: 1 like, 149 views, 0 reposts. Roughly 3.1k stars is the post's figure.
All benchmarks are project reports; private reference audio was not obtained and 0.4 had no listening test. The pinned commit predates this window.

## Sources

- [Post presents Earshot and fit inverse audio synthesis, October 30, 2026 at 22:25:58](https://x.com/i/status/2116174776708616530)
- [Supplementary: pinned October 22 README with fit benchmarks and limits](https://github.com/Leonxlnx/earshot/blob/591fa3e028032e6dce56620a20e932e35667e8d8/README.md)
- [Supplementary: pinned commit date](https://github.com/Leonxlnx/earshot/commit/591fa3e028032e6dce56620a20e932e35667e8d8)

[中文](../earshot-fit-recording-to-parametric-code.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
