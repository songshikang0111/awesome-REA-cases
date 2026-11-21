# Consessus: REA research into four Mac coding apps' local channels connects existing chats

Category: Applications and clients · REA
Record date: 2026-11-21
Stage: In progress

At 08:53:23 Beijing time on November 21, 2026, ns (@ns0bj) introduces the open-source Consessus project: inspect how Claude Code, the Codex desktop app, Antigravity and OpenCode communicate on a Mac, one at a time, then connect existing chats so one app's session can message another and read its answer. The 08:53:44 methods reply explicitly credits the author's reverse-engineering agent rea and identifies Codex's local IPC socket with length-prefixed JSON, the Antigravity language server's Connect-RPC, OpenCode's local HTTP server and Claude Code's peer socket. This is local application interoperability, not retraining four models or recovering their entire source.

The supplementary 08:53:46 thread reply adds a unified session list, sending and reading in one command, same-folder project rooms and bounded discussions. Relevant README sections, the complete compatibility table and protocol notes were also read at pinned commit fd0874fe94457adb0ca0f68eedda40f7f8431c56, dated November 21, 2026 at 09:04:46 Beijing time. These are supplementary project documents, not additional candidates. They report building and testing on one Mac on November 19, then November 20 live send/read round trips for Antigravity, Codex and OpenCode CLI, a four-app room, turn-based discussion and four assigned tasks with four answers. These are project records, not reproductions by this collection.

Version and path distinctions matter. The documented environment is macOS 27.2 on Apple Silicon, Claude Code 2.1.294, Claude Desktop 5.11492.5, Codex desktop 26.1111.71025, OpenCode CLI 2.3.2 and Antigravity app 2.33.0. OpenCode desktop 1.19.5 requires a listener started inside its session and cannot be addressed or have replies read by the unified send command. Thus the post's statement that nothing is installed inside apps is not an exception-free guarantee. Codex CLI terminal sessions, Gemini CLI and Cursor CLI are not covered; the newer path for Antigravity IDE 2.6.0 was not tested live. The direct Claude send/read command itself was not run live, although its reader reportedly ran inside rooms. Free discussion and room lead/set remain fake-only tests.

The project explicitly depends on undocumented local behavior that app updates may change. A socket write, application acceptance, a model reading a message and an actual answer are distinct evidence. Different permission modes can cause recipient holds, denials or expiry; peer data grants no human-instruction authority and changes no application approval mode. Security notes acknowledge that malicious processes under the same OS user are outside the isolation guarantee, and ten hardening tests remain todo. README and compatibility descriptions of some hand-edited room-state boundaries are also not fully consistent, so they do not certify safety. This collection only read sources: it did not install the project, run targets, contact local sessions, inspect credentials or independently verify a round trip. Status remains in-progress.

November 21 sealed snapshot: introduction 0 likes, 24 views, 0 reposts, 1 reply; methods reply 1 like, 26 views, 0 reposts, 1 reply.
Project tests were not run here. Reported live results apply only to the listed versions and one Mac, not all-direction compatibility or security isolation.

## Sources

- [ns introduces cross-app Consessus sessions, November 21, 2026 at 08:53:23 Beijing time](https://x.com/i/status/2123942816397291683)
- [Author identifies rea and four application channels, November 21, 2026 at 08:53:44 Beijing time](https://x.com/i/status/2123942908319424668)
- [Supplementary author reply: session list and project rooms, November 21, 2026 at 08:53:46 Beijing time](https://x.com/i/status/2123942914501853479)
- [Pinned README sections, commit dated November 21, 2026 at 09:04:46 Beijing time; project-reported November 19–20 tests](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/README.md)
- [Complete compatibility table at the same commit: live, untested and known limits](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/docs/COMPATIBILITY.md)
- [Historical local Claude peer-protocol notes at the same commit](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/docs/discovery.md)

[中文](../consessus-rea-mac-agent-app-interoperability.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
