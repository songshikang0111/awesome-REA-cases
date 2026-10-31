# Homecloud photos to Immich: Claude orchestrates private requests and external-drive storage

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-31
Stage: Needs verification

At 05:22:34 Beijing time on October 31, 2026, codila (@0xCodila) describes an integrated Claude Code/Opus 5.5 photo migration: inspect Mac/Windows storage, deploy Docker, open-source Immich and Tailscale, import cloud photos and make another backup. The goal is retaining phone backup and remote browsing while reducing storage subscriptions. At 09:22:08 the same author repeats the workflow. This is self-hosted photo migration, not reimplementation of iCloud or Google Photos services.

The claimed reversing step repeats private cloud-photo webpage requests to download originals, checks N/N against cloud listings and enables phone backup through two QR codes. The earlier post says cloud originals are not deleted; the newer wording 'nothing in your cloud' is not evidence of deletion or successful migration. No actual library size, completed export count, album/Live Photo losslessness report or error log is supplied. N/N is a workflow claim, not acceptance results obtained here.

At 09:06:00, ElioEx (@elioex0) describes the related Homecloud route, naming iCloud-reverse-engineered and giving external-drive parameters, new-install limits and storage estimates. Public lookup located Bodila51/iCloud-reverse-engineered; README and changes were statically read at pinned commit c83ea2685e19b6f924d4cdc628ad5f10cc058f9f, dated October 31 at 04:37:39 Beijing time, before this window. The public workflow matches codila's description, but similar names do not establish that Bodila51 is codila.

The project reuses pyicloud for iCloud authentication/download and Google Photos Toolkit request formats/response parsing for the Google browser path, then imports into Immich. This is not independent recovery of every protocol from scratch. The pinned change passes Mac --upload-location and Windows -UploadLocation through setup: photos may stay on a permanently connected external drive while the database stays on the computer. It applies only to new installs, not automatic migration of existing libraries. Download-then-import usually budgets about 2.2 times the library, with a 100GB example needing about 220GB and backup on another drive. The Mac Photos route additionally needs room for its Photos library; the estimate is not universal.

The README retains important limits: until logout, an iCloud session key can be read by programs running as the same user, so privacy is not absolute. Google private requests may change and entail terms/account risks; Takeout is suggested for users unwilling to accept that risk. N/N cannot detect an incomplete Google webpage listing. Locked Folder, Trash and albums shared by others are excluded; Storage saver supplies only the version Google kept. Mac/Windows Immich deployment has Docker overhead and is not Immich's recommended environment; phone background uploading is OS-limited. The project promises not to alter/delete cloud files; plan downgrades and disabling sync remain user decisions, not automatically safe consequences of promotion.

This update obtains public repository/documentation evidence and corrects the earlier unknown-repository boundary. Full authentication/download implementations were not audited, and no password entry, account access, script execution or migration occurred here. Costs still include drives, electricity and Claude during setup. Free, unlimited and fully lossless operation remain unverified. REA is unspecified.

Earlier snapshot: 42 likes, 1,333 views, 2 reposts. This window: ElioEx 1 like/98 views/0 reposts; codila 50 likes/3,935 views/8 reposts.
N/N and 2.2× storage are workflow/estimate claims, not actual export acceptance results. Static reading only; not run.

## Sources

- [Codila's Claude cloud-photo migration guide, October 31, 2026 at 05:22:34](https://x.com/i/status/2116279618894516660)
- [ElioEx describes Homecloud external drives, new installs and 2.2× storage, October 31, 2026 at 09:06](https://x.com/i/status/2116335848312430784)
- [Codila again describes private-request migration to Immich, October 31, 2026 at 09:22](https://x.com/i/status/2116339908822319428)
- [Supplementary pinned Homecloud README: routes, upstream projects and risks](https://github.com/Bodila51/iCloud-reverse-engineered/blob/c83ea2685e19b6f924d4cdc628ad5f10cc058f9f/README.md)
- [Supplementary external-drive setup change, October 31 at 04:37 Beijing time, before the candidate window](https://github.com/Bodila51/iCloud-reverse-engineered/commit/c83ea2685e19b6f924d4cdc628ad5f10cc058f9f)

[中文](../codila-claude-cloud-photo-immich-migration.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
