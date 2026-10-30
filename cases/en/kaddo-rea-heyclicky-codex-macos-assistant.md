# Kaddo: a public Codex-powered Mac assistant attributed to REA investigation of HeyClicky

Category: Applications and clients · REA
Record date: 2026-10-30
Stage: In progress

At 14:23:15 Beijing time on October 30, 2026, Katleho Nkoe (@kadd_nkoe) says reverse-engineer-anything helped build Kaddo, a HeyClicky-inspired Mac assistant powered by their Codex subscription, choosing open source rather than sales. Public search led to KNkoe/Kaddo's README at e2948ce44ed53bd5f042e5b71bc303bc0527a432, committed that day at 07:12:26 Beijing time, before the window. It confirms observing and reverse engineering the installed app, describing an independent experimental project with potentially different functionality/reliability and no maintenance schedule. This is distinct from baseline author Ayush Pratap's private HeyClicky reconstruction.

The README describes native macOS chat, voice, screen context and background Codex agents. It requires macOS 14, Swift 6, Xcode command-line tools and a signed-in compatible Codex CLI. Background agents also require Apple Silicon, Python 3.12, a local verifier on port 8765, a pinned public Laya model download and network access for installation; they do not run without the verifier. Its implementation and safety were not reviewed here, so its existence is not reliable-action certification.

Voice audio goes to Codex realtime; proactive suggestions can send locally recognized screen text and recent activity to Codex, while chat and attachments use the selected provider. Workspace restrictions are not full filesystem isolation. Screen, accessibility and microphone permissions require user actions; subscriptions do not imply unlimited quotas and third-party services have separate conditions. Copied HeyClicky recordings and third-party logos are omitted; event sounds are currently silent.

Own code declares MIT, with separate dependency/model terms. Documentation lists swift test, but live tests require signed-in tools and can perform real operations. This collection installed nothing, granted no permissions, downloaded no model, started no service and ran no tests. Feature parity and privacy promises remain unchecked; retained as an in-progress public implementation.

Candidate snapshot: 0 likes, 17 views, 0 reposts. Low engagement does not exclude a concrete project.
Pinned commit: 2026-10-29T23:12:26Z. Static README reading only; local verifier and live tests unverified.

## Sources

- [Katleho Nkoe's REA/Kaddo open-source account, October 30, 2026](https://x.com/i/status/2116053300214665282)
- [Pre-window pinned README: experimental status, features, verifier and privacy requirements](https://github.com/KNkoe/Kaddo/blob/e2948ce44ed53bd5f042e5b71bc303bc0527a432/README.md)

[中文](../kaddo-rea-heyclicky-codex-macos-assistant.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
