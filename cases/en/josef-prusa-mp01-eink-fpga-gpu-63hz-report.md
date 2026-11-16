# Minimal Phone MP01: Josef Prusa studies the E-ink FPGA and moves pixel control to the GPU

Category: Hardware and interoperability · REA use unconfirmed
Record date: 2026-11-16
Stage: In progress

At 06:31:06 Beijing time on November 16, 2026, Josef Prusa (@josefprusa) reports modifying the Minimal Phone MP01 E-ink phone. Its original experience reportedly made even Slack difficult, and he stopped using it after a few weeks. After setting up a new development machine, he spent a few days experimenting to improve the display. The goal is making owned hardware useful, not designing a new panel.

He reports building fresh Android, reversing the obscure FPGA driving the E-ink, building a new bitstream-synthesis toolchain, and using a GPU shader to control pixel charge at 63 Hz. He identifies slow FPGA RAM holding the comparison framebuffer as the bottleneck, moving comparison and control logic to the GPU and sending only lighter/unchanged/darker signals over the display interface. Two video attachments accompany claimed 63 'fps' Doom and Sonic demos. This is not a full-panel refresh rate, ghosting measurement or system-wide frame rate measured by this collection.

He connects the experience to modern AI agents lowering the barrier to hardware modification, but names no model, REA use or task-by-task AI contribution. Autonomous agent discovery of the bottleneck is not established. He explicitly lacks time to maintain it or finish a complete Android build, offering to clean it up and publish on GitHub if someone in the MP01 community takes over. Retrieval confirms attribution, full text and attachments only; video behavior, code, bitstreams and hardware were not examined. Retained as in progress, not a released flashable image or universally reproducible phone upgrade.

Sealed candidate: 86 likes, 3,233 views, 1 repost, 9 replies. A few days and 63 fps are author descriptions, not measurements here.

## Sources

- [Josef Prusa on MP01 display research, 63 Hz and code awaiting cleanup, November 16, 2026 at 06:31:06 Beijing time](https://x.com/i/status/2122095073038856334)

[中文](../josef-prusa-mp01-eink-fpga-gpu-63hz-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
