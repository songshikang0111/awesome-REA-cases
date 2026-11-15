# Fireface UCX control on Linux: Johan uses REA and Claude to study the Windows driver, then tests cable by cable

Category: Hardware and interoperability · REA
Record date: 2026-11-15
Stage: Needs verification

At 20:42:10 Beijing time on November 15, 2026, Choblin (@choblin29) reports a Linux driver project for the RME Fireface UCX and follows with a link to Johan Yngman's article dated the same day. The UCX already exposes 18 inputs and outputs in Class Compliant mode. The problem is not total Linux incompatibility, but DSP mixing, EQ, dynamics and reverb settings still depending on Windows TotalMix FX.

Supplementary reading of Johan's November 15 article finds that he used Claude Code with REA to call Ghidra and rizin, inspect the Windows driver and follow USB requests, stream setup and fader commands. The mixer uses a format previously documented for RME FireWire devices; he credits snd-firewire-ctl-services and oscmix rather than attributing every protocol discovery to AI. He says Claude wrote all the code, while he chose a declarative configuration design, pushed for fuzzing, clang-tidy and sanitizers, and spent about a week moving cables, running quiet loopback tones, watching device meters, restarting and testing sleep/resume. This is not an unattended one-shot build.

The article reports the snd-fireface-ucx kernel driver, ucxtui terminal mixer and ucxcfg JSON configuration tool, claiming 18 channels, 32–192 kHz, both MIDI ports, routing, EQ, dynamics, reverb and echo, and 3.5 ms round-trip latency at 48 kHz through PipeWire. These are author results; raw latency logs were not inspected here. The article explicitly says only one first-generation UCX was tested, not a UCX II or the whole product family. It links realbogart/fireface-ucx-linux and states MIT licensing. This collection did not review the full source or license, install a driver, execute the target or connect hardware; status remains unverified.

Main sealed candidate: 2 likes, 499 views, 0 reposts, 4 replies; link reply: 0 likes, 165 views. About one week describes the author's development/testing experience, not AI-only working time.
3.5 ms is the author's round-trip measurement at 48 kHz through PipeWire, on one first-generation UCX.

## Sources

- [Choblin on the UCX driver and hands-on testing, November 15, 2026 at 20:42:10 Beijing time](https://x.com/i/status/2121946863523987476)
- [Same-thread candidate reply linking the original article, 20:42:12](https://x.com/i/status/2121946868976660569)
- [Supplementary Johan Yngman article dated November 15, 2026: REA method, one-unit testing and reported 3.5 ms](https://johanyngman.com/fireface-ucx-on-linux-reverse-engineered-and-built-with-claude-code.html)

[中文](../johan-fireface-ucx-linux-rea-claude-driver.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
