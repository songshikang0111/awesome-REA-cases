# Claude Code third-party APIs: a DeepSeek fallback report, not proof of deliberate degradation

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-02
Stage: Needs verification

At 20:33 Beijing time on November 2, 2026, AI Fun (@ai_funss) recounts DeepSeek reversing Claude Code to investigate capability changes with third-party APIs. The post claims line 280101 removes thinking/effort and retries after rejection, and a Latch mechanism responds to gateway HTTP 400 errors on private parameters by successively dropping deep thinking, structured output, 1M context and Threads without user notification.

The post calls this proof of degradation but supplies no revision, file path, code, parameter names, request/response logs or reproduction. A line number cannot identify a revision. Even if fallback exists, incompatible parameters alone establish neither malicious intent nor reduced reasoning quality. Lookup confirms attribution and an image, not inspected here; the original analysis was not obtained. Retained as a secondary third-party-adaptation investigation, not an established four-stage sequence or effect on all models. REA is unspecified. No gateway credentials were accessed or client run.

Candidate snapshot: 11 likes, 5,139 views, 1 repost. Line 280101, 1M and four-stage fallback are unverified secondary claims.

## Sources

- [AI Fun recounts DeepSeek research into Claude Code fallback, November 2, 2026](https://x.com/i/status/2117233546020667885)

[中文](../deepseek-claude-code-third-party-parameter-fallback-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
