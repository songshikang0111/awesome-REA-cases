# Windows loader: REA and Codex analysis without running the sample

Category: Applications and clients · REA
Record date: 2026-11-08
Stage: Analysis test

At 07:21 Beijing time on October 18, Fedele Mantuano (@fedelemantuano) introduces a Windows loader analysis by asking what can be learned about malware without running it. He reports using REA, Ghidra and Codex to uncover hardcoded servers and in-memory payload loading. A loader is a program responsible for loading a subsequent payload; the purpose here is to understand sample structure and potential communication/loading paths, not actually connect and execute it.

A candidate from this window at 20:57:33 Beijing time on November 8, 2026 relays the experiment again, adding that analysis took place in a Docker lab without network access and explicitly saying the loader was never run. This is a secondary environment description, not a container-isolation audit, malware-escape test or dynamic confirmation. Docker is not equated with a fully secure sandbox.

The available original post provides no sample hash, malware family, function addresses, server values, full evidence chain or decompilation results. The article is only a short link and its text was not obtained. This is therefore the author's reported static analysis. Hardcoded addresses are not established as currently active services, and a possible payload path must not become observed execution. No sample was downloaded or run and no independent reproduction was performed.

October 18 candidate snapshot: 0 likes, 36 views; conclusions are author-reported static findings, not dynamic acceptance results.
November 8 supplementary candidate snapshot: 0 likes, 19 views, 0 reposts. Docker and no-network operation are secondary descriptions; isolation was not audited.

## Sources

- [Fedele Mantuano: static loader analysis with REA/Ghidra/Codex](https://x.com/i/status/2111598581421670782)
- [This window's secondary report: Docker lab without network access and no loader execution, November 8, 2026](https://x.com/i/status/2119414020293943424)

[中文](../windows-loader-rea-codex-static-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
