# Linux reversing-tool smoke tests: Fengshou reports REA 6.8.0 JS analysis and five runnable repositories out of eighteen

Category: Applications and clients · REA
Record date: 2026-11-09
Stage: Analysis test

At 14:00:00 Beijing time on November 9, 2026, 丰收 (@ai_fengshou) says they checked eighteen reversing-tool repositories and could run only five on their Linux machine: REA 6.8.0 completed JS analysis, Frida injection returned data, mitmproxy captured HTTP 200, angr found 228 functions, and all 2,663 Rizin build steps passed. Retrieval confirms attribution, complete wording and an image attachment, not inspection of that image or inferred commands.

The goal is checking runnable toolchain paths in the current environment, not recovering named software. The checks cover analysis, communication, HTTP responses and compilation at unequal depth. HTTP 200 is not reversing correctness, a successful build does not validate Rizin's analysis, and 228 has no known true function count for comparison. No JS target, injected process, scan sample, Linux distribution, dependency versions, commands or logs are supplied. This is not general compatibility or accuracy.

The author explicitly says the other thirteen require environments such as Java, .NET, Windows or paid IDA, and that failure to run locally does not invalidate them. Those environment limits are retained; no missing dependencies were installed here, and the five tools are not all attributed to AI development. REA involvement is explicit only in the JS check. Neither tools nor samples were run by this collection; results remain user-reported smoke checks.

Sealed candidate: 0 likes, 171 views, 0 reposts. Five out of eighteen describes reported local runnability, not analysis success rate.

## Sources

- [Fengshou's eighteen-repository Linux checks and REA 6.8.0 results, November 9, 2026](https://x.com/i/status/2119671326181138707)

[中文](../fengshou-linux-rea-680-reversing-tool-smoke-tests.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
