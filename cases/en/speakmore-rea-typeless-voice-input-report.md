# SpeakMore: REA research on Typeless leads to a voice-input rebuild, with distinct offline and translation limits

Category: Applications and clients · REA
Record date: 2026-11-03
Stage: In progress

At 08:38 Beijing time on November 3, 2026, a Chinese post reports that a Bilibili creator used REA to study Typeless, produced 18 research notes and independently built SpeakMore with hotkey dictation, filler removal, voice translation and selected-text translation. It quotes $144 yearly for Typeless and roughly $1 monthly for everyday SpeakMore use. These are relayed cost claims, not prices or costs measured by this collection.

The README and Typeless overview were read at zephyr4123/speakmore commit edb3ea8b3a1c6933347296f8a963dd529ca21a8b, dated October 30 at 21:31 Beijing time, before the window. They correspond to the named product, 18 notes, macOS/Windows and an MIT declaration, and claim an independent interaction-based implementation without Typeless code. They distinguish direct, hybrid and offline modes: the offline local model only transcribes, without voice translation; selected-text translation always uses the chosen text model. Cost estimates assume 100 uses daily and 26 seconds per utterance, among other conditions. The relayed $1 cannot summarize every configuration.

The overview reports four ordinary-dictation captures on October 13 and six corrections to static conclusions. Translation, HTTP fallback, edit tracking, login and other paths remain dynamically unverified; server models and prompts are unknown. Three-second chunks, WebSocket/HTTP fallback and context capture are project research reports, not server recovery. The README separately reports 1,500 unit tests and 54 installation tests; none were rerun here, and no build or final-package privacy/signature audit was performed. This named public implementation is distinct from the baseline's REATypeless/Saydra and is not forcibly merged.

Candidate snapshot: 2 likes, 241 views, 0 reposts. Costs and tests are relayed/project reports, not independently reproduced.

## Sources

- [Chinese report on SpeakMore, REA and Typeless research, November 3, 2026](https://x.com/i/status/2117415964367024205)
- [Supplementary pinned SpeakMore README, commit dated October 30, 2026, before the window](https://github.com/zephyr4123/speakmore/blob/edb3ea8b3a1c6933347296f8a963dd529ca21a8b/README.md)
- [Supplementary Typeless research overview and dynamic-validation limits at the same commit](https://github.com/zephyr4123/speakmore/blob/edb3ea8b3a1c6933347296f8a963dd529ca21a8b/targets/typeless/docs/00-overview.md)

[中文](../speakmore-rea-typeless-voice-input-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
