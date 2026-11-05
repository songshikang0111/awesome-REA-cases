# Phonon: Elliot uses DeepSeek and Opus for a local Wispr Flow-style dictation rebuild

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-06
Stage: In progress

At 00:53:02 Beijing time on November 6, 2026, Elliot Arledge (@elliotarledge) reports reverse-engineering Wispr Flow, fine-tuning LFM3-1.7B with DeepSeek, and building Phonon with Claude Opus 5.5 [xhigh] as a local alternative to paid dictation. Parakeet transcribes and a refiner cleans up text, both streaming while the user speaks. The target app selects casual Discord, formal Slack/email or Claude Code prompt modes; personal dictionaries can be imported. This is a different author and named project from Vraj's earlier Wispr alternative and is not merged merely because the reference product is the same.

The author reports 65ms from key release to text on an M4 Max versus about 520ms for Wispr Flow on the same clips, and about a quarter second after six minutes of speech. The Rust backend, native Metal fused decode kernel and dflash2 speculative drafter are author descriptions; the drafter was reportedly trained on four local RTX Pro 6000 GPUs. Around 77k public-audio transcripts and synthetic dictations were rewritten by DeepSeek v4.1 flash 1017 in four modes, with no personal dictation used. A Claude Opus blind judge on one hour of lectures preferred Phonon 90 times and Wispr 23. This is not human blind testing, a standard accuracy score or reproduction by this collection, nor evidence of parity for every accent and app.

Supplementary reading covers the public README and license at commit 2e9a5b724845b7b5881701f06c08d00deccc3e5f, dated November 6 at 03:24:41 Beijing time: project material, not another candidate. It specifies 76,960 examples, Apple Silicon and macOS 14+, and about 4.9GB of model downloads plus Python dependencies on first launch. Subsequent dictation is local, but a default daily GitHub update check can be disabled. MLX is the fallback when native engines cannot run. A separate README measurement reports engine-internal median latency falling from 215ms to 30ms over 40 real dictations; that different measure does not replace the 65ms end-to-end claim. Windows remains an unsigned beta using ONNX and a Gemma/llama.cpp CPU path; Mac LFM3/Metal performance cannot be transferred to it.

The README says local history and screen context default off. Microphone, Accessibility and Input Monitoring permissions are needed, with Screen Recording additionally required for screen context. Source is GPL-3.0; weights retain separate licenses. The README identifies Parakeet as CC-BY-4.0 and limits commercial use of the LFM-derived refiner to organizations below $10 million annual revenue. Not every component is unconditionally open for commercial use. Full source, network behavior and training were not audited; nothing was installed, run or rebenchmarked here. Reversing attribution remains the author's claim; a public implementation does not establish recovery of Wispr's internal source. REA is not mentioned.

Sealed candidate: 722 likes, 21,201 views, 43 reposts; higher live metrics do not replace this snapshot. Performance, the 90-to-23 preference and training resources are author/project reports, not independent evaluation.

## Sources

- [Elliot's Phonon/Wispr Flow research and self-test report, November 6, 2026 at 00:53:02 Beijing time](https://x.com/i/status/2118386115170496855)
- [Supplementary pinned Phonon README, commit dated November 6, 2026 at 03:24:41 Beijing time](https://github.com/Infatoshi/phonon/blob/2e9a5b724845b7b5881701f06c08d00deccc3e5f/README.md)
- [Source GPL-3.0 license at the same commit; weight restrictions are in the README](https://github.com/Infatoshi/phonon/blob/2e9a5b724845b7b5881701f06c08d00deccc3e5f/LICENSE)

[中文](../phonon-wispr-flow-elliot-local-dictation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
