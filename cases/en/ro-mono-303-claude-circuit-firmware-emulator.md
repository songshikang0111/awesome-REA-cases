# ro-mono-303: reported Claude-assisted TB-303 circuit/firmware research, with a ROM sequencer and modeled voice

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-03
Stage: In progress

At 22:08:52 Beijing time on November 3, 2026, the candidate congratulates @lemusdev on ro-mono-303's Mac/Windows AU/VST3 beta, crediting Claude Code with circuit and firmware research on Roland's TB-303. The TB-303 is a bass synthesizer with a sequencer; the goal is to preserve sequencing behavior and analog sound in a music host, not merely copy its panel. AI attribution comes from this secondary post; documentation alone does not establish which analysis Claude performed.

Supplementary reading uses Lemus commit 32b3e4961fded5e5298bea45c1c8e19717de499c, dated 17:58:40 Beijing time that day, before this candidate window, solely as implementation context. The docs say the sequencer runs original NEC uPD650C-133 firmware on a uCOM-43 CPU emulation ported from MAME, with pattern RAM, keys, LEDs and CV/gate/accent/slide latches. The voice is modeled component by component from service schematics. The top-level README gives AU/VST3/standalone builds and labels the project early, under AGPL-3.0 with BSD-3-Clause MAME CPU cores. CPU emulation is not presented as AI-created from scratch.

The TB-303 README reports 16/16 service checks and fitting/comparison against 400 single notes from one real unit: a 3.0dB log-spectral distance, versus 2.4dB for the unit's own retakes and 3.3dB for Roland's software. These are project-documented tests, not reruns here or equivalence across all units and sounds. Brightness in the first 100ms remains approximately 25% off. MIX IN, CV/GATE output, the headphone amp and battery LED behavior are not emulated.

The repo supplies no ROM or trademark artwork. Full sequencing requires the user's own legally obtained ROM; without it, MIDI voice mode has no sequencer. Some real-unit recordings and research references are private, limiting independent verification. Only public documentation was read statically. No JUCE, builds, plugins, ROMs or audio rendering were used. Supplementary docs also mention a TR-909, but it is not this candidate's target and does not generate another case.

November 3 candidate snapshot: 1 like, 13 views, 0 reposts. The 16/16 checks, 400 notes and errors are project reports, not tests run here.

## Sources

- [Candidate relays ro-mono-303 and Claude Code, November 3, 2026](https://x.com/i/status/2117620026895405083)
- [Supplementary Lemus README, pinned commit dated November 3, 2026, 17:58:40 Beijing time](https://github.com/lemus-dev/lemus/blob/32b3e4961fded5e5298bea45c1c8e19717de499c/README.md)
- [Supplementary TB-303 implementation, validation and limitations at the same pinned commit](https://github.com/lemus-dev/lemus/blob/32b3e4961fded5e5298bea45c1c8e19717de499c/machines/tb303/README.md)

[中文](../ro-mono-303-claude-circuit-firmware-emulator.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
