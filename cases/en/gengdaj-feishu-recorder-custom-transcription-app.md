# BeanScribe: REA-assisted D3200 recording in a self-hosted Feishu transcription app

Category: Hardware and interoperability · REA
Record date: 2026-11-04
Stage: In progress

At 16:38:14 Beijing time on November 4, 2026, Yichen (@gengdaJ) reports researching a recorder and building a Feishu bottom-navigation app with custom UI, features and transcription providers. He quotes about CNY 0.15/hour for StepFun and CNY 1/hour for Doubao real-time transcription. His 19:56:00 post explicitly credits REA, names BeanScribe and describes physical-button recording, a handshake, Bluetooth streaming, captions, post-recording recognition and Feishu documents, using an existing lightweight server. Prices and success are author reports, not total deployment costs.

Supplementary README, third-party and release-validation documentation is pinned to mcncarl/beanscribe commit ea731f311302bfb17dd1700a99976cb768358716, dated November 4 at 16:19:27 Beijing time, before both candidates. It identifies the Soundcore D3200. The project explicitly reuses tacshi/Soundcore's protocol documentation and real-time-stream implementation. Its own work includes Feishu H5/JavaScript Bluetooth sessions and WebCrypto, a Python gateway, StepFun/Doubao adapters, a recording library and private documents. The attribution document reports additional checks of file listing, deletion, response matching, authentication rejection and audio offsets in a Feishu Android 8.3.6 Soundcore SDK sample; upstream commands and cryptography are not claimed as original discoveries. REA conversations and step-by-step tool output were not publicly checked.

The README specifies single-user private deployment, not replacement of native Feishu Miaoji captions, changes to official ASR quotas or automatic shutdown of factory transcription. The post reports a 2–3-second handshake; documentation for tested firmware 04.92 warns that roughly the first 2–4 seconds may not reach the web app. Later recognition processes saved audio and cannot automatically recover that gap. Stopping reception in the web UI may leave the device recording; its physical button must end recording. A floating window does not establish unlimited iOS background recording. Configured speech, summary and translation providers receive data; self-hosting is not offline operation. The author found no flashing method, and hardware-start behavior changes remain unfinished.

Release documentation reports 229 frontend tests, 149 backend tests and checks of 97 release files using synthetic audio and local mocks, not tests rerun by this collection or real ASR/Feishu-document validation. The original implementation has iPhone/D3200 acceptance experience, but the generalized release was not fully retested on another user's tenant and device. Its source-available license permits free personal noncommercial use while requiring written authorization for internal organizational business and commercial use; it is not OSI open source, and upstream rights need separate checking. This collection only read public documentation, without installation, hardware access, flashing, service calls or credential access.

Sealed first-post snapshot: 41 likes, 5,346 views, 3 reposts; follow-up: 1 like, 122 views, 0 reposts. Prices, delays and test counts retain their distinct source contexts, not independent reproduction.

## Sources

- [Yichen's first report: recorder app, pricing and limitations, November 4, 2026 at 16:38:14 Beijing time](https://x.com/i/status/2117899207764062606)
- [Same-author REA/BeanScribe workflow follow-up, November 4, 2026 at 19:56:00 Beijing time](https://x.com/i/status/2117948976624189462)
- [Supplementary project README pinned to November 4, 2026 at 16:19:27, before the candidates](https://github.com/mcncarl/beanscribe/blob/ea731f311302bfb17dd1700a99976cb768358716/README.md)
- [Third-party protocol attribution at the same revision](https://github.com/mcncarl/beanscribe/blob/ea731f311302bfb17dd1700a99976cb768358716/THIRD_PARTY.md)
- [Release-validation scope at the same revision, separating mocks from hardware experience](https://github.com/mcncarl/beanscribe/blob/ea731f311302bfb17dd1700a99976cb768358716/docs/VALIDATION.md)

[中文](../gengdaj-feishu-recorder-custom-transcription-app.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
