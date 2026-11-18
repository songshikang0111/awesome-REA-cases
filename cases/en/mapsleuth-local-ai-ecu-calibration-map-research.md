# MapSleuth: Robbie studies ECU calibration maps with local AI on two DGX Sparks

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-19
Stage: In progress

At 01:08:07 Beijing time on November 19, 2026, Robbie Searles (@rsearles35) introduces MapSleuth, which he is building. An ECU is an automotive electronic control unit; calibration maps hold parameter mappings used in control behavior. The project aims to find and decode these maps in ECU firmware using local AI on two DGX Sparks. No vehicle, ECU model, firmware revision, particular map or AI model is supplied. This does not establish completed or safe vehicle tuning.

The author says he has moved the model backend from vLLM to TensorFold, with output rising from approximately 40 to 57 tok/s and first-token latency falling from approximately 1.25 to 0.18 seconds. These are reported inference measurements in his environment, not map-recognition accuracy, decoding completeness or vehicle performance. Test conditions and repeated-run data are absent.

Retrieval confirms attribution, complete wording and date. Images, source, firmware samples and logs were not reviewed, and no model was run or vehicle accessed. Retained as an in-progress project; REA is unmentioned. No ECU-writing, vehicle-safety-bypass or road-tuning instructions are provided.

Sealed candidate: 3 likes, 55 views, 0 reposts, 2 replies. Throughput and first-token figures are author reports, without an ECU-recognition benchmark.

## Sources

- [Robbie's MapSleuth and local-inference migration report, November 19, 2026 at 01:08:07 Beijing time](https://x.com/i/status/2123100953595240836)

[中文](../mapsleuth-local-ai-ecu-calibration-map-research.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
