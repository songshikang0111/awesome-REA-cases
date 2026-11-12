# GoGra on Linux: four decompiler errors and two AI errors in a Ghidra/OpenCode workflow

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-12
Stage: Needs verification

At 10:22:02 Beijing time on November 12, 2026, Takashi Yoshikawa (@MalwareBibleJP) summarizes Fortinet researchers' analysis of Linux GoGra, also reportedly presented at Black Alps 2026. GoGra exchanges commands through Outlook mail. The target is a stripped Go payload embedded in a PDF-disguised dropper, not a replacement mail client. The reported workflow connects an LLM to Ghidra through MCP alongside OpenCode; neither a model nor REA is identified.

According to the summary, the LLM wrote a Ghidra script to recover function names from .gopclntab and identify the OUTLOOKCLIENT package. Researchers catalogued six errors. Four concern the decompiler: omitting getpid (where the AI's comment was correct), omitting a SendingMessages call, incorrect argument counts and incorrect Go-string boundaries. The latter two are attributed to handling 32-bit x86 Go stack-based calling conventions and non-NUL-terminated strings. The two AI mistakes were claiming that GetClientName returns Linux rather than a username, and confusing the dropper's Go build ID with a Graph API bearer token. An AES-use inference also lacked evidence until the researcher requested the mail-processing code; this is not counted as a seventh classified error.

The post also relays a behavioral chain: OAuth 2.0 obtains a Graph API token, messages with subject Input are read and deleted, Base64 and AES-CBC processing precede Bash execution, and encrypted results return in Output messages. This is a defensive analysis summary, not a payload or executable exploitation procedure. Six observations from this study are not a general error rate.

This collection checked the original post's text and attribution but did not read its linked primary article, conference material, sample, scripts or complete analysis output. Technical conclusions remain attributed to this secondary account. AI and decompilers potentially correcting one another does not establish automatic verification. No malware was downloaded or executed, and no mail service was contacted.

Sealed November 12, 2026 snapshot: 2 likes, 326 views, 0 reposts. Four decompiler errors and two AI mistakes are relayed research findings, not independent retests.

## Sources

- [Takashi Yoshikawa's GoGra Linux six-error summary, November 12, 2026 at 10:22:02 Beijing time](https://x.com/i/status/2120703635630051540)

[中文](../gogra-linux-ghidra-opencode-six-errors-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
