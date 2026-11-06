# Jungle Outpost: Pizza Yap reconstructs Peekcell's pixel style and acknowledges falling short

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-06
Stage: Analysis test

At 23:32:29 Beijing time on November 6, 2026, Pizza Yap (@pzayap) says they reverse-engineered Peekcell's art style, explicitly crediting the original as designed rather than prompted with ChatGPT Image 2.6, and admits their result is not as close or as good. The post attaches a video and publishes a complete prompt for Jungle Outpost, an interactive pixel diorama in one HTML file. It does not recover Peekcell's original project files or prompt.

Reading the full prompt shows concrete constraints: a 230×230 offscreen art-pixel canvas, nearest-neighbor scaling to a visible canvas at most 920px wide; string pixel maps, a shared palette and no antialiasing, gradients or blur; and oblique buildings with front, top and right faces in different shades, with side depth 25–35% of front width. The scene includes a container outpost, satellite dish, tent, temple tower and trees, with ten characters and specified idle/click actions.

Interaction requirements include alpha-based pixel hit testing with 1px tolerance, topmost-character priority, one requestAnimationFrame loop, a MET 0/10 counter, sequential triggers about every 1.7 seconds, arrow-key selection and Space/Enter activation, phone taps and reduced-motion preferences. No external images does not mean fully offline: the prompt separately requests Google's Press Start 2P font. These are generation requirements, not a validated implementation checklist.

Retrieval confirms authorship and a video attachment, but the comparison was not watched, HTML read or interactions executed. The model that ran the prompt is unspecified; Image 2.6 is not assigned as the execution model. The author's admission of falling short is retained, without a quantitative similarity score. No generation was rerun here and REA is not mentioned. Publishing the prompt does not transfer rights to the original art or assets.

Sealed candidate: 1 like, 97 views, 0 reposts. All dimensions and character counts are prompt requirements, not runtime acceptance results.

## Sources

- [Pizza Yap's full Jungle Outpost style-reconstruction prompt and self-assessment, November 6, 2026 at 23:32:29 Beijing time](https://x.com/i/status/2118728231608275313)

[中文](../pizza-yap-peekcell-jungle-outpost-style-prompt.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
