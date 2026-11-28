# Replacing a stimulation patch's app: Shashank credits Claude with BLE research and a Flutter client

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-28
Stage: Needs verification

At 14:47:17 Beijing time on November 28, 2026, Shashank Mayya (@ShashankMayya) says a purchased vagus-nerve stimulation patch has good hardware but an app with sessions dying on screen lock, broken login and failed health syncing. The author credits Claude with helping reverse-engineer its Bluetooth protocol and build a replacement client. Brand and model are unspecified; neither a medical/consumer manufacturer nor identity with a separate microcurrent self-experiment post is inferred.

Supplementary posts by the same author at 14:47:18–14:47:24 say no documentation, SDK or API existed. The author decompiled the Flutter app's Dart code with blutter and matched it against Bluetooth logs in logcat. Reported protocol properties include three writes to start, two to stop, four bytes converted to battery voltage and opposite byte orders for duration writes and timer readback. The five-year-session statement illustrates a misinterpretation risk; it is not a calculation or device operation performed by this collection.

The Flutter replacement reportedly stays on the phone without login or backend, with four modes, favorites, history, reminders, live battery and reconnection. The main repair is foreground-service session persistence with Pause, Mute and Stop in notifications. A mode named migraine reportedly gives the patch a ten-second timer for each on-phase so output stops if the app dies. Other reported features include fading soundscapes, pausing that stops stimulation, resuming at level 1 and voltage-based charging inference. Health Connect displays 30 days of sleeping heart rate and nights with versus without sessions. Samsung Health reportedly syncs about two hours late and does not share HRV, so the app displays waiting-for-data status and checks again. Chart associations do not establish health benefits from stimulation.

The author reports restricting intensity to the official table, starting at level 1, avoiding unknown characteristics and the firmware channel, and testing off-body first, plus over 200 tests and Patrol end-to-end runs on a real device. These are stated engineering constraints and test counts, not a certified safety protocol or test results verified here. Source, protocol captures, test reports and brand specifications were not obtained. Attachment details were not inspected, no device was connected and nothing was reproduced. Current, dosage, failure protection, medical suitability, efficacy and data privacy cannot be confirmed; local-only operation was not independently audited. REA is unmentioned.

November 28, 2026 sealed candidate: 0 likes, 28 views, 0 reposts, 1 reply. The same-author thread is supplementary evidence, not five independent verifications.

## Sources

- [Window candidate: Shashank introduces the Claude/BLE stimulation-patch client, November 28, 2026 at 14:47:17 Beijing time](https://x.com/i/status/2126568596281426137)
- [Same-author supplement: blutter decompilation and logcat comparison, November 28, 2026 at 14:47:18 Beijing time](https://x.com/i/status/2126568599305462248)
- [Same-author supplement: background sessions and ten-second device timer, November 28, 2026 at 14:47:21 Beijing time](https://x.com/i/status/2126568613012545581)
- [Same-author supplement: Health Connect's 30-day heart-rate comparison, November 28, 2026 at 14:47:22 Beijing time](https://x.com/i/status/2126568617051607055)
- [Same-author supplement: over 200 tests and device Patrol runs, November 28, 2026 at 14:47:24 Beijing time](https://x.com/i/status/2126568624051913053)

[中文](../shashank-vagus-patch-claude-ble-flutter-app.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
