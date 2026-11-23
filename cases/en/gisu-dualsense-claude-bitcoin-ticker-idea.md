# A DualSense BTC ticker: gisu shares a Claude Code lightbar and trigger-control prompt

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: Needs verification

At 05:47:11 Beijing time on November 23, 2026, gisu (@0xGisu) says Claude Code reverse-engineered a personal PS5 DualSense into a Bitcoin ticker: the lightbar goes green or red with price direction and R2 stiffens as the price falls. A prompt is offered as something readers can make in about thirty minutes. The concrete design is a Windows Python application using the existing pydualsense library over USB, polling the free CoinGecko BTC API every ten seconds. The prompt requests light color relative to one minute earlier, brightness proportional to movement, both motors rumbling for one second after a move greater than 0.5% in five minutes, R2 resistance following the 24-hour change, player LEDs indicating that change in 1% steps, and touchpad presses printing price and change in the terminal.

Original-post retrieval confirms the author and a video attachment, but the video was not watched, generated code was not obtained, and controller behavior, API limits and individual effects were not tested. Retained as a concrete AI implementation idea and author report about hardware reuse. Calling an existing controller library does not establish that the author or Claude newly decoded the DualSense protocol; prompt requirements are not automatically tested features. Thirty minutes is not an auditable duration, and REA is unmentioned. No dependencies were installed or price API accessed here.

Sealed snapshot: 1 like, 62 views, 0 reposts, 1 reply. Video not watched; thirty minutes is a promotional claim.

## Sources

- [gisu's DualSense ticker report and full Claude Code prompt, November 23, 2026 at 05:47:11 Beijing time](https://x.com/i/status/2124620733267464627)

[中文](../gisu-dualsense-claude-bitcoin-ticker-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
