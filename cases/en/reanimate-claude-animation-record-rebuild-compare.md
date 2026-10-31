# reanimate: a public Claude Code skill for recording, rebuilding and comparing animations frame by frame

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-31
Stage: Analysis test

At 10:02:00 Beijing time on October 31, 2026, Agent Skills Hub (@agentskillshub) introduces NiazMorshed2007/reanimate in a skills roundup, claiming frame-by-frame Claude Code reversing of any animation with identical verification. Supplementary reading used README at commit 522a353be364828ef43e1440faf5c1077edccbc1, dated October 30 at 10:31:21 Beijing time, before the candidate. Documentation and project measurements do not make 'any' or 'identical' universal guarantees.

The aim is overcoming one-shot screenshot-based rebuilding that cannot see motion errors. The skill records a website, screen recording, mp4, gif or Lottie reference at a fixed viewport and frame rate, capturing video, per-frame element positions and CSS/Web Animations data. It specifies each element/property's duration, start/end values, easing and stagger, implements with the target project's existing CSS, Framer Motion, GSAP or three.js, records the copy in the same way and compares timing, curves and pixels. It describes usually two to five rounds and reports remaining differences after five with reasons rather than always claiming success.

The default matches motion with an 80ms timing tolerance; exact-look mode additionally requires at most 2% mean pixel mismatch. Public examples cover Stripe cards, WorkOS, Clerk, Liveblocks, Resend and others, reportedly mostly taking 30–80 minutes. Stripe card examples claim 0.03% pixel difference at rest and tilt within 0.4px. These are project measurements, not reruns here. Canvas/WebGL paths record GPU calls, shaders, uniforms and scene graphs, using a virtual clock and seeded randomness to reduce capture variance. This can also read original assets and code, so it is not described as a guaranteed no-source-copying clean room.

Documentation requires Bun 1.1 or newer on macOS/Linux; Windows is untested. Only Claude Code is reported tested; other-agent compatibility is unproven. Login pages, YouTube and Loom require supplied recordings rather than direct capture. Workers' own clocks remain real-time; particles use blurred distribution comparisons when the reference random generator cannot be reproduced, not pointwise equality. Linux hardware-GPU capture is untested. Fonts, images and code retain their owners' rights. No dependencies were installed, target sites opened, assets captured or skill executed here. Universal equivalence, safety and permission are not established. REA is unspecified.

Candidate snapshot: 0 likes, 50 views, 0 reposts. The roundup reports 101 stars; not functional evidence.
80ms, 2%, 0.03%, 0.4px and 30–80 minutes are project-documentation figures, not independently retested.

## Sources

- [Agent Skills Hub's roundup entry for reanimate, October 31, 2026](https://x.com/i/status/2116349940666703976)
- [Supplementary pinned reanimate README: example measurements, comparison thresholds and limits, October 30, 2026](https://github.com/NiazMorshed2007/reanimate/blob/522a353be364828ef43e1440faf5c1077edccbc1/README.md)

[中文](../reanimate-claude-animation-record-rebuild-compare.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
