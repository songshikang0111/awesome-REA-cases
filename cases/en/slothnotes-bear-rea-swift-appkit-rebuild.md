# SlothNotes: Shakirul studies Bear with REA before rebuilding a Swift/AppKit notes app

Category: Applications and clients · REA
Record date: 2026-11-13
Stage: Needs verification

At 13:18:50 Beijing time on November 13, 2026, Shakirul (@shakirul) reports building SlothNotes with AI in about a week: a Bear-inspired Swift/AppKit notes app with no third-party dependencies and an MIT license. Bear is the existing notes application he studied. He explicitly credits @morluto's REA skill for studying behavior before rebuilding piece by piece, describing it as copying behavior, not code. An author reply at 13:30:05 distinguishes this from screenshot-based imitation, and another at 13:31:14 supplies a repository link. These replies are supplementary sources, not additional candidates or achievements.

Supplementary GitHub discovery located KhanShaheb34/SlothNotes; the account's public twitter_username is shakirul and its name is Shakirul Hasan Khan. The project README, MIT license and Bear migration documentation were read. Pinned revision d93510f9313168fb881e8129905a7dc3be220ac9 was committed on October 21, 2026 at 06:10:17 UTC, before this report, so the documents are not described as a November 13 release. The README calls the app Sloth and describes a three-pane Markdown editor, tags/wiki links, attachments and Quick Look, search, archiving and import/export, local storage and optional iCloud Drive exchange. It requires macOS 13 or later.

The documentation explicitly says a complete iCloud round trip between two physical Macs has not been verified; automated sync tests simulate local folders. Concurrent edits become conflict copies and history has no automatic cleanup. There is no iPhone/iPad app, files are not encrypted, and local builds are not notarized. A separate Bear migration tool is documented as taking read-only snapshots of the database, WAL and attachments, checking the source is unchanged before import, preserving note states and using backups, a ledger and conflict copies to avoid overwrites. These are inspected designs and test scopes, not data-safety validation by this collection.

The license text confirms MIT, but about a week remains the author's estimate, without audited sessions, hours or behavioral equivalence. The model, Bear version, REA investigation addresses and itemized comparisons are not supplied; a complete Bear clone is not established. No target code was downloaded or executed, no notes library accessed, and no build or tests run here. Public implementation and project documentation are not independent reproduction.

Sealed candidate: 6 likes, 224 views, 0 reposts, 8 replies. About a week is author-reported, not audited working time.

## Sources

- [Shakirul's REA/Bear behavior study and SlothNotes report, November 13, 2026 at 13:18:50 Beijing time](https://x.com/i/status/2121110519868207263)
- [Supplementary author reply: behavior study rather than screenshots, November 13, 2026 at 13:30:05 Beijing time](https://x.com/i/status/2121113348779409504)
- [Supplementary author repository reply, November 13, 2026 at 13:31:14 Beijing time](https://x.com/i/status/2121113636588454088)
- [Pinned README: features, macOS requirements and physical iCloud limitations; revision committed October 21, 2026](https://github.com/KhanShaheb34/SlothNotes/blob/d93510f9313168fb881e8129905a7dc3be220ac9/README.md)
- [Pinned MIT license text](https://github.com/KhanShaheb34/SlothNotes/blob/d93510f9313168fb881e8129905a7dc3be220ac9/LICENSE)
- [Pinned Bear migration design and test-scope documentation](https://github.com/KhanShaheb34/SlothNotes/blob/d93510f9313168fb881e8129905a7dc3be220ac9/docs/bear-migration.md)

[中文](../slothnotes-bear-rea-swift-appkit-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
