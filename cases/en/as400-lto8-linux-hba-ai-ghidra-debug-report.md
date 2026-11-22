# LTO8 migration and Linux HBAs: an author credits AI and Ghidra with a tape-device kernel-crash fix

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: Needs verification

At 02:57:05 Beijing time on November 23, 2026, @desitechsuppoat describes exchanging LTO8 tapes with clients mainly using IBM AS/400 systems to migrate about 100 TB, much of it scanned images. Replacement parts for old standalone drives are difficult to obtain, and rack libraries do not directly replace that migration step, requiring loans of the author's drives. The author reports modifying AS/400 to accept non-original drives and repairing incomplete Linux HBA (host bus adapter) modules and tape configuration after module initialization.

AI reportedly identified gaps while the author wrote C prototypes/pseudocode and comments in Emacs, manually reserving device opcodes and loading/calling orders unknown to the model. The agent then generated surrounding logic, tested, iterated and requested human approval, reportedly taking five rounds to learn the intended workflow. Complete-post retrieval supplies the outcome: drives reload after ejection, but power loss could not be simulated, so a smart plug let Claude exercise actual off/on transitions and HBA behavior over two full days. The author says CCB (command control block) problems caused at least one hundred kernel traps the previous month; the last was found and fixed the previous week with AI-assisted kernel debugging and Ghidra.

These are retrospective author claims, not measured work all occurring during this post. Five rounds are not five projects and 100 TB is not verified throughput. No device models, kernel revision, patches, Ghidra analysis, transition matrix or test logs are supplied. Universal drive compatibility, independence from vendor support and end-to-end reliability are unestablished. Retained as an unverified legacy-device interoperability and debugging report, omitting unrelated discriminatory remarks. No smart plug, kernel or tape device was operated here; REA is unmentioned.

Sealed post: 4 likes, 250 views, 0 reposts, 1 reply. Two days, five rounds and at least one hundred kernel traps are author reports; no patches or logs were obtained.

## Sources

- [Author's long reply on AS/400, LTO8, AI/Ghidra and HBA debugging, November 23, 2026 at 02:57:05 Beijing time](https://x.com/i/status/2124577927656313316)

[中文](../as400-lto8-linux-hba-ai-ghidra-debug-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
