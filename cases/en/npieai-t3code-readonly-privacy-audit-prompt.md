# T3 Code privacy-audit idea: NpieAI's read-only source checklist for an agent

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-27
Stage: Needs verification

At 11:14:10 Beijing time on November 27, 2026, NpieAI (@NpieAI) publishes a reusable prompt for AI to perform a read-only privacy/outbound audit of a local fork or clone of pingdotgg/t3code. The author describes using self-built source versions and wants to know whether the actual build sends data to third parties other than model APIs or reads unnecessary files. The same-thread 11:13:06 parent supplies this motivation only; its allegations about the telemetry dispute are not findings verified by this collection.

The checklist first identifies the version and local changes, then asks about #42299, #42465, #42380, #42450, #42356, #42629 and community patch #43026 or an equivalent change. These are the author's proposed checks, not confirmation that patches merged or their descriptions were reviewed here. It traces fields through product-telemetry directories, ID hashing, switch priority and when identity reads occur, distinguishing confirmed, possible and not found with file/line references. Further checks cover usage logs, identity-file and keychain access, OpenTelemetry, relay tracing, remote access, feedback, crash reporting, Antigravity quota probes, automatic updates, web/mobile clients and installation scripts.

The author prohibits file changes, builds and dependency installation, requesting a channel/risk table, prioritized change locations and runtime network/file-read verification methods. Read-only source inspection alone cannot prove that a running binary never sends data. Credential paths in the text are code references to investigate, not authorization for an agent to open a user's actual credentials. This entry preserves a behavior-research/audit proposal, not audit output, build hashes, packet captures or file-access records. It concludes neither that T3 Code leaks data nor that it is safe or its switches reliable. No model or REA is specified. This collection read no real credentials, executed no prompt and did not audit the target repository.

Sealed candidate: 0 likes, 40 views, 0 reposts, 0 replies. A checklist is not an audit result; no PR or runtime data was validated.

## Sources

- [NpieAI's complete T3 Code read-only privacy/outbound audit prompt, November 27, 2026 at 11:14:10 Beijing time](https://x.com/i/status/2126152573786992855)
- [Supplementary same-thread self-build context and motivation, November 27, 2026 at 11:13:06 Beijing time; disputed claims unverified](https://x.com/i/status/2126152307427692937)

[中文](../npieai-t3code-readonly-privacy-audit-prompt.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
