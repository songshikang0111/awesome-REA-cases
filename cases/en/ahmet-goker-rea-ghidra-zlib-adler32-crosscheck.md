# zlib Adler-32: Ahmet Göker cross-checks constants, assembly and six inputs with REA

Category: Algorithms and feature recovery · REA
Record date: 2026-11-07
Stage: Analysis test

At 17:44:30 Beijing time on November 7, 2026, Ahmet Göker (@_shadowintel_) describes trying REA and Ghidra on a real zlib library. The target is identifying and checking Adler-32 checksum computation, not rebuilding the compression library. A function search found both forwarding code and the actual implementation with the same name, prompting the author to distinguish addresses and follow the calculation body.

The author compares decompiled constants 65521 and 5552 with source, examines assembly and checks computed results for six different inputs. Ghidra reportedly typed a function's return as void; comparison with assembly and source suggested a different real type. The concrete lesson in the report is treating decompilation as an interpretation to check rather than stopping at names or constants. Function addresses, corrected type, six input values and a result table are not supplied in the post. Neither test vectors nor the affected function are invented here.

Retrieval confirms attribution and four image attachments, but their outputs were not read and the link was not expanded. zlib revision, architecture, sample hash, scripts and replayable logs were not obtained. Six-input checking is author-reported, not independent reproduction by this collection or proof of equivalence on all inputs. The older GhidraMCP constant-filtering case does not establish the same analyst or sample, so this remains separate. No tools or target were run here.

Sealed candidate: 0 likes, 180 views, 0 reposts. Six-input results and the return-type correction were not independently checked.

## Sources

- [Ahmet Göker reports REA/Ghidra zlib cross-checks, November 7, 2026 at 17:44:30 Beijing time](https://x.com/i/status/2119003046470390239)

[中文](../ahmet-goker-rea-ghidra-zlib-adler32-crosscheck.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
