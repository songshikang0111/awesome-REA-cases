# When curl.exe retries: Nate Brooks reports Claude/REA analysis checked against source and a server

Category: Applications and clients · REA
Record date: 2026-11-27
Stage: Analysis test

At 03:57:42–03:58:25 Beijing time on November 27, 2026, Nate Brooks Crypto x AI (@NateWeb3AI) describes installing the REA skill in Claude Code and providing Windows curl.exe without accompanying source, asking which HTTP errors trigger --retry and how long it waits. The full thread identifies the target rather than leaving it as an unnamed EXE. The author reports eight tool calls searching for a retry message, following it into an unnamed function, decompiling and finding its caller, and interpreting hexadecimal constants as HTTP codes.

The reported codes are 408, 429, 500, 502, 503, 504, 522 and 524, with an initial one-second wait doubling to a ten-minute cap, overridden by Retry-After, plus separate rules for timeouts, refused connections and FTP. The author says comparison with open-source curl found all eight codes and constants matching; a local test server produced waits of 1, 2 and 4 seconds for 503, two seconds each for 429, and no retry for 404. Two seconds for 429 describes that test, not a universal fixed delay.

These are author-reported static analysis and dynamic comparisons, not this collection's reproduction. The target version, binary hash, full tool logs, matching source revision and server script were not obtained; image attachments were not inspected. Source absent from the input does not make curl closed source or establish that the model never saw its public implementation. General platform support and 263-tool promotion do not establish success on other targets. No REA installation or target execution occurred here; analysis-test retains these evidence limits.

Sealed opening post: 0 likes, 5 views, 0 reposts, 2 replies. Eight calls and 8/8 matches are author reports, not independent reproduction.

## Sources

- [Nate's opening curl.exe analysis post, November 27, 2026 at 03:57:42 Beijing time](https://x.com/i/status/2126042733659734397)
- [Same-thread target and question, 03:57:43](https://x.com/i/status/2126042737698803766)
- [Same-thread eight-tool-call workflow, 03:57:44](https://x.com/i/status/2126042740735787200)
- [Same-thread retry codes and wait rules, 03:57:44](https://x.com/i/status/2126042743084298467)
- [Same-thread author report of source/server comparisons, 03:57:45](https://x.com/i/status/2126042746763051025)

[中文](../nate-brooks-curl-retry-claude-rea-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
