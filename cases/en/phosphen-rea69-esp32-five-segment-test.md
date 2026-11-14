# An ESP32 firmware test: Phosphen says REA 6.9 split five segments and verified checksum and SHA-256

Category: Hardware and interoperability · REA
Record date: 2026-11-12
Stage: Analysis test

At 04:48:26 Beijing time on November 12, 2026, Phosphen (@phosphenq) reports an ESP32 firmware-image test in a post about a build from REA's 6.9 release branch. The tool reportedly split the image into five segments and verified its checksum and SHA-256. This is a specific firmware-container parsing and integrity-check report, not decompilation of five modules or reconstruction of flashable firmware.

No device model, image origin, hash values, segment addresses, reference parser or verification output is supplied. Five segments do not mean five partitions, and no vulnerability or application logic is inferred. UF2, Intel HEX, Motorola S-record and U-Boot support are also listed, but without concrete inputs and results for them; a format list is not counted as testing.

Retrieval confirms text and attribution. The video, repository revision and sample were not reviewed, and the 6.9 designation and build origin remain author statements. This is a separate target from the same post's own-app exposure test, sharing the source without treating whole-post engagement as separate popularity. This collection downloaded no image, executed no REA, recomputed no target checksum and flashed no device.

Whole-post November 12, 2026 snapshot: 29 likes, 755 views, 0 reposts. Five segments and successful verification are author reports, not independently recomputed.
Supplementary pinned Espressif docs (October 1 commit, before the candidate) describe variable data segments, a footer checksum and an optional SHA-256 for corruption detection. The simple hash is distinct from a secure-boot signature; it does not establish publisher identity, code safety or success of this REA test.

## Sources

- [Phosphen's ESP32 five-segment and integrity-verification report, November 12, 2026 at 04:48:26 Beijing time](https://x.com/i/status/2120619685582401814)
- [Supplementary Espressif image-format docs, committed October 1, 2026 at 22:21:27 Beijing time; statically read November 12 only to explain segments and integrity checks](https://github.com/espressif/esptool/blob/8aefcacb19cd100e23754d7a166d29015c4ba22c/docs/en/advanced-topics/firmware-image-format.rst)

[中文](../phosphen-rea69-esp32-five-segment-test.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
