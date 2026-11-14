# rea-toon: agent-assisted shot, character and script analysis of short dramas, with VIDEO.md exports

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-14
Stage: Related project

At 23:13:14 Beijing time on November 14, 2026, the candidate introduces JuneYaooo's new rea-toon project: give an AI agent local short-drama videos to study scripts, characters and production shot by shot. It does not reverse a video player or recover a filming project file. Built on rea-video's shot cutting and voice/music separation, it adds a narrative layer and is recorded separately from the existing rea-video entry. The public English README was read at pinned commit d94acc1, dated November 14 at 14:31:41 UTC (22:31:41 Beijing time). This earlier documentation is supplementary evidence, not another candidate.

Documentation describes shot splitting and subtitle OCR, character merging, assigning each line's speaker, resolving disagreements against frames, reading scenes, eyelines, dramatic beats and information gaps, then using code to count pacing, emotion ledgers and screen time. Outputs are study/script/shot-script pages and a VIDEO.md plus video directory package. Scripts and shot scripts can export to PDF, and clicking a shot replays that point in the original. Cross-episode views examine character arcs, setups/payoffs, episode-end hooks and paywall points. These are project descriptions, not proof of accurate identification of every character, speaker or reason for popularity. Code counts model-assigned emotion tags, not objective emotional ground truth.

The project distinguishes live action, AI live action, 2D/3D animation, motion/meme comics and commentary. It requires Python 3.10+, ffmpeg and a vision-capable agent or API, including Claude Code and Codex. About 30 vision calls per episode is a documentation estimate; trying five episodes first is a budgeting recommendation, not a cost or speed measured here. Input must already be on disk; links are not downloaded. Series use one file per episode and reportedly support resumption. Pages and reports currently primarily output Chinese; the English demo was translated separately and does not establish complete English output support.

The README names PolyForm Noncommercial 1.0.0 and requires written author permission for commercial use. The LICENSE text was not separately reviewed and video rights were not obtained; tool licensing grants no rights to source dramas. This collection only read pinned documentation, without watching the demo, installing dependencies, running the CLI or checking output. Included as a specific AI-assisted content-study tool with related-project status, not conflated with morluto's REA or software decompilation.

Sealed candidate: 6 likes, 319 views, 0 reposts, 3 replies. About 30 vision calls per episode and trying five episodes first are project budgeting guidance, not rerun here.

## Sources

- [Introduction to rea-toon shot-by-shot short-drama study, November 14, 2026 at 23:13:14 Beijing time](https://x.com/i/status/2121622492171378964)
- [Supplementary pinned README: features, evidence replay and noncommercial limits, commit November 14, 2026 at 14:31:41 UTC](https://github.com/JuneYaooo/rea-toon/blob/d94acc1a4523d97651b6076730b42dcdf2a9bcc5/README.md)

[中文](../rea-toon-short-drama-shot-script-analysis-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
