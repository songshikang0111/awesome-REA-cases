# Messages API to Rust: HenryPeng relays Claude reconstruction and anonymous difference-fingerprint verification

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-26
Stage: Needs verification

At 21:24:55 Beijing time on November 26, 2026, HenryPeng (@HenryPeng123) discusses what he identifies as a November 25 Anthropic engineering article by Lance Martin and colleagues. It describes migrating the Messages API used by customers, Claude Code and Cowork from Python to Rust, with Claude drafting the core request path in about a week. This is a source-available behavior-preserving migration case, not cracking a private service or recovering unknown original source.

The post says April tests passed about 98%, while only roughly a quarter of production inputs matched. About 700 integration tests already existed, and an audit found over 100 weakened assertions in ported tests. Python kept changing, model replies were nondeterministic, and customer requests/replies could not be read. The model was therefore called once and its output replayed to Rust. Checkpoints and fingerprints captured the first divergence and length shapes rather than raw payloads. Agents synthesized inputs from fingerprints in a sandbox, iterating with a sub-second input check requiring no model call, then checking whether the fingerprint disappeared in production shadow traffic.

Human acceptance remains explicit: in mid-May an agent copied a missing web-search tool description into files, passing local comparisons, but an engineer still required the real internal-service call. The April chart compares inputs only, with replies compared separately; comparison scope changed and six misleading days were excluded. The post reports production traffic switching in September, about 70% less CPU per request and about 20% lower median time to first token. However, the seven-day CPU average covers one region, memory covers all production with no percentage stated, and TTFT covers a shorter Claude Code traffic window. The decline before the first plotted point mostly occurred on Python, so it cannot all be attributed to Rust. The claim that Claude wrote over 80% of code merged by Anthropic by May is not this project's AI-code share.

Retrieval confirms the author and full post, but the article short link was not expanded. The original article, source, production fingerprints, test output and raw performance data were not obtained; the poster also explicitly did not reproduce the work. Dates, figures and methods remain this secondary interpretation, not certification of production correctness, privacy or safe deployment. No code, customer data or service was accessed or run. REA is unmentioned.

Sealed snapshot: 2 likes, 164 views, 0 reposts, 0 replies. About one week, 98%, one quarter, 70% and 20% are relayed figures, not remeasured.

## Sources

- [HenryPeng's account of the November 25 Anthropic migration article and statistical limits, November 26, 2026 at 21:24:55 Beijing time](https://x.com/i/status/2125943885981446362)

[中文](../anthropic-messages-api-rust-shadow-parity-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
