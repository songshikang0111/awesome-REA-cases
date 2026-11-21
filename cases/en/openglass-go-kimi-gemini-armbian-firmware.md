# OpenGlass Go: Kimi researches a glasses-free 3D display; Gemini finishes replacement Armbian firmware

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-22
Stage: In progress

At 02:03:56 Beijing time on November 22, 2026, Megabits (@Megabits_mzq) reports porting full Armbian, adding decoding patches and finding a mainline kernel driver bug to submit later. Supplementary posts at 01:51:36 and 01:58:00 identify Looking Glass Go, a glasses-free 3D display, and the OpenGlass Go project. The author describes Orange Pi-like internals with H618, SD storage and an STM32 controlling display and power. Kimi is credited with most reversing and early code, Gemini Neon with the final stretch. Time saved is not quantified; finding a bug is not upstream acceptance.

Public Builder/Apps READMEs and lkg-mcu docs were read. Builder revision 5ca6710 dates to November 22 at 01:04:25; Apps revision df77557 to November 21 at 21:56:58. These are original commit dates, not additional candidates. Docs describe an ARM64 image with pinned Armbian, Linux 6.18.63, U-Boot and Debian Trixie, DRM/KMS apps, 3D image/video pre-rendering, file management and Mac USB storage mode. lkg-mcu documents serial calibration reads, Linux-online notification, power-off and USB/standalone switching. These support the concrete interoperability direction; implementation and protocol traces were not audited.

The projects claim AI assistance, real-hardware tests and human design review; Apps even labels its code 100% AI-written. These are project attributions, not contribution audits. Builder docs explicitly distinguish static image checks from device tests. Original SD media and data should be preserved; third-party firmware risks malfunction and warranty loss, and combined components retain separate licenses. No image was downloaded, build executed or device flashed. Media compatibility, decoding behavior and the driver bug remain unverified; status is in-progress.

Sealed candidate: 0 likes, 76 views, 0 reposts, 0 replies. Only the supplied candidate is judged; the thread and repositories are supplementary evidence.

## Sources

- [Megabits on Kimi/Gemini, Armbian and decoding patches, November 22, 2026 at 02:03:56 Beijing time](https://x.com/i/status/2124202164860150025)
- [Supplement: OpenGlass Go announcement and device background, November 22, 2026 at 01:51:36 Beijing time](https://x.com/i/status/2124199061767221414)
- [Supplement: H618, SD and STM32 structure, November 22, 2026 at 01:58 Beijing time](https://x.com/i/status/2124200670786134462)
- [Builder README pinned to the November 22 at 01:04:25 commit, read later](https://github.com/megabitsenmzq/OpenGlass-Go-Builder/blob/5ca67100645fc09d6de8fa217067ec0f37124890/README.md)
- [Apps README pinned to the November 21 at 21:56:58 commit, read later](https://github.com/megabitsenmzq/OpenGlass-Go-Apps/blob/df775577dd9f361c17c0bbcb3918e9598e4cef99/README.md)
- [STM32 serial-tool documentation at the same Apps revision](https://github.com/megabitsenmzq/OpenGlass-Go-Apps/blob/df775577dd9f361c17c0bbcb3918e9598e4cef99/lkg-mcu/README.md)

[中文](../openglass-go-kimi-gemini-armbian-firmware.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
