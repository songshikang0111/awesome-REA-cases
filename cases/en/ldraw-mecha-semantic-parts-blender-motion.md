# LDraw Mecha: infer LEGO mechanisms from parts text, then map them to Blender animation

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-08
Stage: Related project

At 05:17:00 Beijing time on November 8, 2026, Xiao Tan (@tvytlx) introduces antelocnova's LDraw Mecha: infer mechanical subassemblies and coupling from part descriptions and placement text, map annotations onto glTF nodes, then rig and animate with Blender Python. The goal is animating mechanisms in existing static LEGO CAD, not merely generating new bricks from prompts. The candidate describes the 42043 truck being too complex, leading Claude Sonnet to suggest animating only its pneumatic crane, a reduced scope accepted by the author.

Supplementary reading of the linked author's Show HN description, originally posted at 03:41:20 Beijing time on November 7, confirms anteloc/ldraw-mecha and v0.5.0. The tag's README, Gallery and validation document were read; GitHub's API resolves it to c09ad90caf4f4cba00b1542eb622de8e580e8498, committed at 00:55:19 Beijing time on November 8. These are supplementary project documents, not additional window candidates or independent tests. README separates annotated .mpd research, submodel/mechanism inference, motion planning, conversion to matching annotated .glb and Blender-script generation. Samples credit Sonnet 5.5 and Opus 5.5 and retain the 42043 scope reduction. Gallery also lists 42000 steering/differential/V8 and separate 42083 mechanisms.

Validation distinguishes declared motion, Blender implementation and saved animation. Transform comparisons, mixed poses, reopening, sampled clearance and human visual review are not interchangeable. --require-reviewed can include explicit deferrals and does not discover missing mechanisms. Clearance sampling does not establish continuous collision freedom, containment or non-worsening of existing contacts. The tool implements declared rigid-body kinematics, not guarantees about forces, friction, backlash, general closed-loop/contact solving or flexible-material physics. The 10265 v2 example leaves doors, rear ride-height adjustment, gearshift and supercharger unimplemented; corrected contact discovery does not retroactively validate an old rig.

Python 3.12+ is required. README calls Linux x86_64 and Windows/WSL2 paths WIP and untested. The candidate's no-physics-engine and hose limitations remain attributed to that account; supplementary docs provide more precise boundaries. Smooth animation is not physical feasibility, nor do selected author examples prove automatic success for arbitrary models. No dependencies were installed, target or tests run, or videos watched here. REA use is not claimed.

Sealed candidate: 0 likes, 205 views, 0 reposts. Low circulation does not erase project value; documentation review is not reproduction.
The tag's resolved commit predates the candidate. Only public text was read; project tests were not executed.

## Sources

- [Xiao Tan introduces LDraw Mecha and the 42043 scope reduction, November 8, 2026 at 05:17 Beijing time](https://x.com/i/status/2119177320703357172)
- [Supplementary author Show HN project description, November 7, 2026 at 03:41:20 Beijing time, before this window](https://news.ycombinator.com/item?id=50397325)
- [Supplementary pinned README: v0.5.0 resolves to the November 8, 00:55:19 Beijing-time commit](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/README.md)
- [Same-commit Gallery: model/animation listings, not videos watched here](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/GALLERY.md)
- [Same-commit validation: kinematics, coverage and physical limits](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/docs/validation.md)

[中文](../ldraw-mecha-semantic-parts-blender-motion.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
