# Diyar Persian keyboard: M.A.H reports AI-assisted review after decompilation

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-04
Stage: Needs verification

At 20:40:31 Beijing time on November 4, 2026, M.A.H (@DevUranium) reports decompiling the Diyar Persian keyboard assistant amid controversy and using AI to explain its architecture. He describes extracting a WiX Burn installer, inspecting its MSI database, opening cab1/cab2/cab3 and recovering C# from .NET 9 binaries, with plans to publish on GitHub for review. Retrieval confirms authorship and text, not a confirmed repository or analysis artifacts; a publication plan is not publicly available source.

He reports SetWindowsHookEx/WH_KEYBOARD_LL, Named Pipes and TSF events, saying CoCoTextService.dll enters other processes as a text service. He calls password-field filtering heuristic and fragile and claims files lack Authenticode signatures. He characterizes this as high-risk dual-use architecture that could buffer passwords. Importantly, the post explicitly says AI did not identify a Trojan, ransomware or information stealer. The author found no secret servers, password exfiltration or hidden webhooks, reporting only update checks and Azure translation when users configure their own keys.

These are the author's and his AI's static interpretations, not this collection certifying safety or maliciousness. TSF and keyboard hooks alone do not establish eavesdropping, password leakage or infection of every process. Versions, hashes, permission paths, runtime captures, signature-check results and independent audits are absent. Cited source line numbers are author locators, not checked here. The model and REA use are unspecified. Images were not inspected, decompiled code was not downloaded and the program was not run.

Sealed snapshot: 0 likes, 11 views, 0 reposts. Both the Riskware label and absence-of-exfiltration judgment are author opinions, not independent forensic findings.

## Sources

- [M.A.H's Diyar decompilation and AI architecture analysis, November 4, 2026](https://x.com/i/status/2117960180906275128)

[中文](../diyar-persian-keyboard-ai-decompilation-security-review.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
