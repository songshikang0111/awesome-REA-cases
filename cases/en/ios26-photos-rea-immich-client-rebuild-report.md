# iOS Photos to an Immich client: reported REA inventory of 226 actions, 147 implemented and 85,000 media items

Category: Applications and clients · REA
Record date: 2026-11-11
Stage: In progress

At 19:30:07 Beijing time on November 11, 2026, uudon (@uudonX) relays a user unfamiliar with iOS development moving 85,000 photos/videos to Immich to avoid iCloud subscriptions and retain server ownership. Dissatisfied with third-party clients, the user reportedly asks Claude to rebuild familiar Photos behavior. Unlike the existing Homecloud private-request migration case, the target is a new Immich client informed by Apple Photos behavior.

The account says Claude Code and REA study iOS26.3 Photos frameworks and enumerate 226 actions, including copying edits, hiding, cover selection, dragging into albums and Spotlight search. One agent writes only behavioral descriptions, which guide implementation in an effort to avoid copying Apple code. Claude writes code and UI tests, runs the simulator and compares screenshots; the user sets scope, tests daily on an iPhone and reports mismatches. Early crashes/stalls with 85,000 items reportedly improve after repeated hardware tuning. The account says 147 actions currently work and most remaining ones depend on iCloud.

Server-hosted originals, cached phone timelines/thumbnails, offline browsing, automatic new-photo backup, deletion allowed only after backup confirmation, and communication solely with the owner's server are relayed design/features, not audited network or deletion safety. The 226 is an inventory denominator and 147 is not an independently passed-test count; omissions are not all established as impossible. Retrieval confirms the commentator and text. Original developer, repository, license, specifications, test coverage, devices, performance and migration records were not confirmed. Open-source and clean-room claims are not elevated into legal-compliance findings. The closing dialogue about avoiding model refusals provides no verifiable research result and is not propagated as a technique. This collection read no private photos, connected to no server and built no client.

Sealed snapshot: 0 likes, 63 views, 0 reposts. 85,000, 226 and 147 are reported figures, not checked against the original project.

## Sources

- [uudonX's iOS Photos/REA/Immich client reconstruction account, November 11, 2026 at 19:30:07 Beijing time](https://x.com/i/status/2120479178369978791)

[中文](../ios26-photos-rea-immich-client-rebuild-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
