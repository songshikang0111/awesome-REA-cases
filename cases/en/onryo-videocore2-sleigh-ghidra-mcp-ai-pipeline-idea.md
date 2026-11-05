# A VideoCore II firmware idea: add SLEIGH decoding before AI analysis through MCP

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-05
Stage: Needs verification

At 05:01:45 Beijing time on November 5, 2026, Onryo (@3r1k4dl3r) proposes passing a firmware blob through a custom VideoCore II SLEIGH decoder, then Ghidra, MCP and a frontier AI for automated reverse engineering, followed by independent validation and iterative refinement. SLEIGH supplies Ghidra with a processor-instruction specification; MCP connects the agent to analysis tools. Connecting a model does not itself supply missing instruction decoding.

A supplementary thread read finds a root posted at 23:14:11 on November 3 discussing whether a Raspberry Pi is secure for signing Bitcoin transactions, with ynniv questioning its binary blobs. At 04:44:15 on November 5, ynniv says Ghidra does not even handle VideoCore2 and most tools do not, prompting Onryo's pipeline suggestion. At 05:14:43, ynniv says work is already underway but is not REA. These supplementary posts establish context and tool attribution, not additional candidates or proof that ynniv implemented Onryo's entire proposal.

Firmware revision, SLEIGH source, instruction coverage, decompilation samples, model and validation logs are absent. Independent validation is a requirement in the idea, not verified firmware analysis, evidence of a backdoor or assurance about a Raspberry Pi signing environment. Kept as an unverified concrete idea. No firmware was downloaded or executed, and no wallets or keys were handled.

Sealed candidate: 0 likes, 21 views, 0 reposts. Root-post engagement does not replace the candidate snapshot.

## Sources

- [Candidate: Onryo's VideoCore II/AI pipeline, November 5, 2026 at 05:01:45](https://x.com/i/status/2118086322003030235)
- [Supplementary root: Raspberry Pi transaction-signing context, November 3, 2026 at 23:14:11](https://x.com/i/status/2117636465811468353)
- [Supplementary parent: ynniv on missing VideoCore2 decoding support, November 5, 2026 at 04:44:15](https://x.com/i/status/2118081917320872084)
- [Supplementary reply: ynniv says work is underway but is not REA, November 5, 2026 at 05:14:43](https://x.com/i/status/2118089581258064097)

[中文](../onryo-videocore2-sleigh-ghidra-mcp-ai-pipeline-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
