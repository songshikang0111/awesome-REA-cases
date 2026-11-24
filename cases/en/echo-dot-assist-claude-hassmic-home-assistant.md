# echo-dot-assist: Claude helps replace Alexa while keeping an old Echo's microphones and wake engine

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-24
Stage: In progress

At 08:09:25 Beijing time on November 24, 2026, Michael_AI_Hu publishes an article about connecting an idle Echo to a home assistant, introducing Julian Imhof's echo-dot-assist. The full article and README at revision 7489169, dated 09:32:18, were read. This within-window revision is supplementary documentation, not another candidate. The goal is to reuse an Amazon Echo's far-field microphones, original audio processing and wake engine, replace its Alexa client with the small hassmic daemon, retain Fire OS and expose an ESPHome voice satellite to Home Assistant.

The README explicitly says the author wrote code, notes and documentation in conversation with Claude. That does not mean Claude independently reversed all firmware. MediaTek exploits, kaeru and TWRP ports for obtaining device control are credited to R0rt1z2; unlocking must be manual and model-specific. Earlier researchers' work is not reassigned to AI. Documented features include local multi-device answer arbitration, timers, announcements, follow-ups, LAN Drop In, Music Assistant multiroom playback, Bluetooth and button/light-ring automation. Wyoming mode provides only a subset including voice, wake words, buttons and music. Echo Show text overlays and Wi-Fi motion sensing remain experimental; sound detection is less reliable. These are project descriptions, not hardware tests by this collection.

The support table lists Dot 2/3, Echo 2, two generations of Show 5/8 and Input, with manual installation only for Dot 5. Appearance does not establish support for every generation: 2019–2020 Dot 3 C78MP8 and clock model 36EBT3 are explicitly unsupported. The author tested only one unit per model and the code is unaudited. Unlocking and system-partition writes wipe the device and can brick it; some models need soldering and specified firmware. The main unlocking path requires physical Linux with direct USB. Windows starts with an already-unlocked device; the article says no complete fresh-device Windows path has been reported.

No Amazon communication is a firewall design goal, not demonstrated zero egress. The article warns that stock daemons may issue DNS requests and response/music addresses come from Home Assistant or Music Assistant. The README admits firewall or update mistakes may expose the device online or on the LAN; before Home Assistant enrollment, other LAN users can connect. The public README was read, not all source or device pages. No unlocking, flashing, installer execution, hardware connection or isolation test occurred here. MIT licensing for original code does not license Amazon firmware, libraries or wake models. This is a different repository from LibreEcho and is not merged with that case. REA is unmentioned.

Sealed candidate: 0 likes, 96 views, 0 reposts, 0 replies. One unit per model is the project's test scope, not independent reproduction or large-scale reliability validation.

## Sources

- [Michael_AI_Hu's echo-dot-assist article, November 24, 2026 at 08:09:25 Beijing time](https://x.com/i/status/2125018915772477502)
- [Supplementary first-party README: Claude credit, single-unit tests, support and risks; 7489169, November 24, 2026 at 09:32:18 Beijing time](https://github.com/Gamer92000/echo-dot-assist/blob/7489169851ac0e196ac0a8647cef2b80ca1f716b/README.md)

[中文](../echo-dot-assist-claude-hassmic-home-assistant.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
