# Partial ransomware-file recovery: a report of Claude analyzing 16KB headers and salvaging formats

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-05
Stage: Needs verification

At 22:16:58 Beijing time on November 4, 2026, Lyren_o (@0xAIlabs) replies to @macintosh_busy praising AI-assisted study of partial ransomware encryption for file recovery. Retrieving the explicit parent finds macintosh's 21:22:35 retelling: someone kept 700 files locked since 2019. Opus 5.5 initially judged per-file AES under RSA infeasible to decrypt, then comparisons with a few clean copies reportedly showed only each file's first 16KB encrypted. The parent supplies context, not another task candidate, and neither the victim nor an original report was confirmed.

The retelling describes roughly a week of format-specific recovery modules from JPEG to MP4, a U-Net trained on an RTX 4070 to repair photo colors, and a new SketchUp parser reconstructing a 239MB model in Blender. A final pass reportedly recovered about 100 more files. Results are stated as 26% fully restored, 27% opening with damage, 12% salvaged and 35% lost. Per-file records and criteria are absent; inferred image reconstruction is not original-byte recovery.

A new account at 09:45:00 Beijing time on November 5 says the agent consulted open documentation to write the SketchUp parser and identified three undocumented structures from bytes. For photo repair it reportedly erased the first 16KB of intact images to create a training set, then trained a U-Net for color restoration. The post compresses outcomes to 65% usable again and 35% lost without stratified validation. That cannot replace the earlier distinction between 26% full, 27% damaged and 12% salvaged. Names, offsets and parser code for the three structures are absent. Its caveats about sub-16KB files and fully encrypted files are this account's claims, not universal recovery rules for ransomware families.

The target is unencrypted remnants and format structure, not breaking AES/RSA, recovering keys or decrypting everything. Ransomware family, samples, code, clean copies, checksums, training logs and recovered files were not obtained. Counts are not inferred from percentages and the percentages are not reproduced success rates. No video was watched, malware run or private files read; REA is not mentioned.

Earlier sealed candidate: 0 likes, 13 views, 0 reposts. Parent-post outcomes are secondhand, not independent recovery evidence.
November 5 sealed candidate: 2 likes, 966 views, 0 reposts. 65% usable does not mean 65% lossless recovery; three undocumented structures remain unchecked.

## Sources

- [Candidate: Lyren_o on AI partial-encryption recovery, November 4, 2026 at 22:16:58 Beijing time](https://x.com/i/status/2117984454593380720)
- [Supplementary parent: macintosh relays 700 files and recovery proportions, November 4, 2026 at 21:22:35; not a candidate](https://x.com/i/status/2117970767476359443)
- [New candidate account: three SketchUp structures, training set and 65% usability, November 5, 2026 at 09:45:00](https://x.com/i/status/2118157601364197459)

[中文](../macintosh-claude-partial-ransomware-file-recovery-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
