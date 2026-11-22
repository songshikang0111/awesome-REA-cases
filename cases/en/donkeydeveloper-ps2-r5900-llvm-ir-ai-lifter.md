# PS2 R5900 to LLVM IR: Donkey Developer reports phased AI implementation and first rendering

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-23
Stage: In progress

At 02:18:51 Beijing time on November 23, 2026, Donkey Developer (@DonkeyDeveloper) says the project is public and explains the AI workflow: the author sets goals and phases, has the model implement and test changes, then feeds logs and results back through many iterations, especially for reverse engineering. Supplementary reading of the pre-window November 22 posts at 18:00:40 and 18:52:11 identifies PlayStation 2 R5900/Emotion Engine (EE) MIPS code as the target, with a plan to lift MIPS into LLVM intermediate representation and eventually C. The author says work began eleven days earlier and first rendering arrived after a week of preparation, crediting GPT-6.2 Sol and hundreds of EE tests in GitHub CI, while explicitly saying the C stage has not been reached.

The earlier reply describes a custom disassembler, opcode decoder, control-flow analyzer and LLVM IR lifter, referencing hardware documentation and PCSX2 for accuracy, with LLVM providing verification and native code generation. These earlier posts establish target and stage, not additional in-window candidates. A repository is offered through a link, but its code, CI artifacts, test inventory and rendering screenshot were not reviewed here. No game, execution platform or full compatibility scope is supplied. First rendering and hundreds of tests are author reports, not proof of complete game playability, exact original-source recovery or autonomous decompilation. No project, target or dependencies were executed here; REA is unmentioned.

In-window reply snapshot: 0 likes, 5 views, 0 reposts, 0 replies. Eleven days, one week and hundreds of tests are the author's figures; CI was not checked.

## Sources

- [Author explains AI goals, phases, tests and log feedback, November 23, 2026 at 02:18:51 Beijing time](https://x.com/i/status/2124568307198300248)
- [Pre-window supplement: MIPS-to-LLVM-IR work and first rendering, November 22, 2026 at 18:00:40 Beijing time](https://x.com/i/status/2124442933248274433)
- [Pre-window supplement: custom R5900 analysis chain and references, November 22, 2026 at 18:52:11 Beijing time](https://x.com/i/status/2124455899721056521)

[中文](../donkeydeveloper-ps2-r5900-llvm-ir-ai-lifter.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
