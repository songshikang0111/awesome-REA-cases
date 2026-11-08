# Photos to an exploded coffee grinder: AI Workflow Lab's Claude/Blender reconstruction

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-08
Stage: Needs verification

At 04:57:19 Beijing time on November 8, 2026, AI Workflow Lab (@AIWorkflowX) shares Claude Is Your 3D Modeler: Build Any Object From a Parts List. Supplementary retrieval obtained the associated article text: using manual coffee-grinder photos, Claude separates 11 parts, estimates millimeter dimensions, connections and vertical positions, and writes Blender Python for separately named geometry, materials and an exploded animation. A 10-part chair illustrates the same method with XYZ separation. This infers structure from photos for explanatory animation, rather than decompiling Blender.

The guide requires checking estimated dimensions and suggests repair diagrams for hidden mechanisms. It explicitly calls the grinder a simplified explanatory design, not a manufacturing model. Corrections include moving the body sideways by 90 mm and shifting the shaft to expose the burrs. Checks cover part count, floating/intersecting geometry, scale, explosion and return. The basic example is 150 frames/five seconds; the reported automated run is 240 frames and a 12-second 1920×1080 video. Those are not combined into a frame rate for one render. The author says desktop Claude operated Blender and edited the video while the human only installed it and approved access, exporting each part's screen coordinates on every frame for tracking labels.

Reported failures include eight simultaneous Blender instances and waiting half an hour after mistaking a finished 286 KB video for an incomplete render. Without scale, photo dimensions are guesses; organic shapes, long multipart scripts, versioned APIs and fixes disturbing other parts can fail. Retrieved text leaves some tables, code or media positions without complete content; no missing script was invented. The finished video was not watched and no code was run here. Geometric accuracy, automation extent and manufacturing feasibility are not established.

Sealed candidate: 12 likes, 708 views, 2 reposts. Ten to fifteen minutes for a specification is guide advice, not timing measured here.

## Sources

- [Candidate and associated grinder/chair modeling article, November 8, 2026 at 04:57:19 Beijing time](https://x.com/i/status/2119172367360344536)
- [Supplementary article: part specifications, Blender animation and reported failures](https://x.com/i/article/2119160344329240576)

[中文](../aiworkflowx-claude-photo-grinder-blender-exploded-view.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
