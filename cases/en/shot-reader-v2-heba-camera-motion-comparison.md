# Shot Reader v2 camera inference: Heba AI reports B-25 miscaptioning and missed handheld shake

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-24
Stage: Analysis test

At 17:12:28 Beijing time on November 24, 2026, Heba AI (@SubarcticRec) provides specific error feedback under an introduction to Shot Reader v2. The supplementary Machine Delusions post, dated 03:43 that day in Beijing, describes inferring camera, lens, blocking and set from a shot as JSON for rebuilding in Blender, claims it can distinguish zoom from camera movement, and calls the weights open under Apache 2.0. These are introduction-post claims only; weights, source and license were not read.

Heba AI judges it worse than Claude + REA: shot 001's push-in at 0.98 confidence and CG style are correct, but the caption calls parked B-25 bombers jets. Shot 013 has a gun-barrel point of view and handheld-style shake, yet is classified as static and not handheld, while REA flags handheld movement. This is a user's comparison of two concrete observations, not a benchmark from which overall accuracy can be computed. The 0.98 is model confidence, not 98% correctness.

The input film, model revision, parameters, Claude model, exact REA configuration and complete output are unavailable. No footage was watched, scene rebuilt or test rerun here. The reply may mean rea-video, but says only REA, so its engine is not asserted and this is not turned into verification of a separate independent tool. The target of the record is Shot Reader v2's visual production-parameter inference test, retaining analysis-test status and attribution.

Sealed candidate: 0 likes, 17 views, 0 reposts, 0 replies. Two observations do not establish overall performance.

## Sources

- [Candidate: Heba AI reports two shot errors and compares Claude + REA, November 24, 2026 at 17:12:28 Beijing time](https://x.com/i/status/2125155581157589254)
- [Supplementary parent: Machine Delusions introduces Shot Reader v2, November 24, 2026 at 03:43 Beijing time](https://x.com/i/status/2124951870032798187)

[中文](../shot-reader-v2-heba-camera-motion-comparison.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
