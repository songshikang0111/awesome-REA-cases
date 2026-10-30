# B2B portal data: SaasNext reports a browser agent reading raw JSON through CDP

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-30
Stage: Needs verification

At 15:31:52 Beijing time on October 30, 2026, SaasNext (@Saasnext_db) compares headless browser agents with direct backend API reversing. Its agent reportedly logs into a vendor portal and listens to Chrome DevTools Protocol's Network.responseReceived events to capture raw JSON rather than scraping rendered HTML tables. The concrete use is recovering structured data inputs from an authenticated, observable business interface, reducing dependence on pixel recognition; it does not establish backend-source recovery or permission bypass.

The author reports 640 ms p95 response time and zero OCR hallucination, but supplies no timing boundaries, sample size, network/hardware environment, portal identity, agent/model, comparison baseline, code or logs. Avoiding OCR removes errors from that step, not necessarily JSON omissions, incorrect business mappings or all agent hallucinations. Model responsibilities are unspecified, so no model capability or REA use is invented. This collection checked the original post only, without logging into a portal, capturing traffic or running an agent. Retained as an unverified agent-interface observation/reconstruction workflow report.

Candidate snapshot: 0 likes, 2 views, 0 reposts. The 640 ms and zero-OCR-hallucination claims were not measured independently; model responsibilities are unclear.

## Sources

- [SaasNext's CDP extraction and 640 ms p95 account, October 30, 2026](https://x.com/i/status/2116070565358305716)

[中文](../b2b-browser-agent-cdp-json-api-observation-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
