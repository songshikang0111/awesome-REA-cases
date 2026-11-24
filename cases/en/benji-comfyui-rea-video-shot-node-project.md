# Shot-by-shot video analysis in ComfyUI: Benji AI announces a single node inspired by rea-video

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-25
Stage: In progress

At 19:41:15 Beijing time on November 22, 2026, Benji AI (@AIfutureBenji) announces shot-by-shot video reverse engineering in ComfyUI with a video attachment. A follow-up at 19:41:49 specifies a single ComfyUI custom node implementing the rea-video idea. ComfyUI is a node-workflow environment. The concrete target is integrating shot-structure analysis into that workflow rather than requiring a separate video-analysis entry point.

These two pre-window sources form one node project, not two additions. Earlier thread retrieval confirmed attribution, parent/reply relation and a 1920×1080 video attachment. The video was not watched, and code, node name, model, input/output schema, installation materials and tests were not obtained. The rea-video idea is the author's inspiration credit, not proof of upstream source reuse or calls to morluto/rea. It establishes neither automatic recreation of full films, validated output quality nor coverage of all video production in one node.

An in-window candidate at 05:26:00 on November 23 by Prince does AI (@princedoesai) describes Rea Video Breakdown for ComfyUI as splitting videos into shots, writing a prompt for each and measuring camera motion with optical flow. Retrieving the original confirms attribution and a photo attachment; the image and short-link destination were not read. This is archived as supplementary discussion of the same ComfyUI shot-analysis goal. No repository, author relationship or version identifier confirms its precise correspondence to Benji's single node. Optical flow is a participant's feature description, not reviewed source code or comparison results, and does not retroactively expand the original announcement's proven scope. Status remains in-progress; no node was installed or video analysis run.

The two older sealed snapshots are 0 likes/32 views and 1 like/15 views; both have 0 reposts, with 1 and 0 replies respectively. An attachment does not establish reproduced functionality.
November 23 supplementary discussion snapshot: 0 likes, 56 views, 0 reposts, 1 reply. Optical flow, per-shot prompts and version correspondence were not checked.
A new candidate at 22:35:31 Beijing time on November 23, 2026 names ComfyUI-ReaVideoBreakdown, describing per-shot analysis by a local vision-language encoder, optical-flow pan speed and zoom rate, VIDEO.md-style reports, JSON and English/Chinese prompts. It claims no external API calls, audio analysis, on-screen text reading or subtitle export; ordinary SD1.5/SDXL CLIP cannot see frames. MIT licensing, two dependencies and features are secondary claims. Repository, code and exact correspondence to Benji's version remain unchecked; nothing was installed or run. Sealed snapshot: 0 likes, 14 views, 0 reposts, 0 replies.
A new account at 00:29:05 Beijing time on November 25, 2026 names benjiyaya's ComfyUI-ReaVideoBreakdown: HSV histograms/pixel differences for cuts; Lucas–Kanade optical flow plus RANSAC for horizontal/vertical pixels per second, zoom percentage per second and static/smooth/handheld classification; VIDEO.md, JSON, per-shot prompts and keyframe previews. It adds a second node combining a breakdown with up to nine reference images into a MiniMax H3 Ref2VA subject-swapping prompt, and claims MIT licensing. A prompt node is not video generation by this tool. Source, revision, input/output and measurement error were not checked, nor precise correspondence with Benji's announcement. Earlier audio, text-reading and subtitle exclusions are retained; their omission here is not an upgrade. Sealed candidate: 1 like, 139 views, 0 reposts, 0 replies. The same post's other two projects go to their existing records, not three independent tests.

## Sources

- [Benji AI's ComfyUI shot-analysis announcement, November 22, 2026 at 19:41:15 Beijing time](https://x.com/i/status/2124468246489477576)
- [Benji AI's follow-up specifies one node and the rea-video idea, November 22, 2026 at 19:41:49 Beijing time](https://x.com/i/status/2124468390576414723)
- [Prince does AI describes ComfyUI per-shot prompts and optical-flow camera-motion measurement, November 23, 2026 at 05:26:00 Beijing time](https://x.com/i/status/2124615403095601301)
- [Secondary account of ComfyUI-ReaVideoBreakdown features and exclusions, November 23, 2026 at 22:35 Beijing time](https://x.com/i/status/2124874492736577951)
- [ComfyUI optical flow and second prompt node in a three-tool account, November 25, 2026 at 00:29:05 Beijing time](https://x.com/i/status/2125265457892536420)

[中文](../benji-comfyui-rea-video-shot-node-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
