# DESIGN:OS Studio: an independent desktop studio that used REA to reverse-engineer Figma .fig files and reimplement the editor

Category: Applications and clients · REA
Record date: 2026-11-10

DESIGN:OS Studio is a local desktop design studio published by Jang Trịnh (jangtrinh). The public repository is https://github.com/jangtrinh/design-os-studio. The README at reviewed commit df14c593e86edcc039adc2c67067bf8db64e9e84 (release v0.7.11) states that it reads Figma .fig containers (fig-kiwi, DEFLATE or Zstd), writes container version 106, and reimplements editor behaviour locally. A bundled designos-mcp server serves tools over stdio. The README's generated tool table lists 39 tools, and selected layers can be turned into CSS, Tailwind, React, SwiftUI, UIKit, Compose, Android XML or HTML. The repository also describes more than 6,000 tests on macOS CI.

Public specs in the same commit set the rule that reverse-engineering of Figma fields uses `rea` (morluto/rea). E1-4 (2026-10-18) records that `rea` (morluto/rea 6.7.0, `npx -y rea-agents`) ran analyze-javascript-application over extracted editor JavaScript (evidence `ev_2624766…`). Wasm lanes were unavailable (WABT and Ghidra were not installed), so the schema was decoded with a roughly 40-line local kiwi decodeBinarySchema reader. plans/261017-figma-parity-wave-ab/rea-findings.md states that the method included static `rg` and REA. plans/reports also contain completed rea inspect-macho and analyze-javascript-application output, and some failed invocations. The product README does not mention REA. Maintainer Jang Trịnh confirmed on 2026-11-10 that REA was used for this Figma work.

The license is PolyForm Shield 1.0.0: source-available, not an open-source license. A known issue documented in the README, #834, remains open: saving a .fig file drops numbered-list formatting and writes inherited or variable-bound paints on instances as fixed values.

This collection reviewed the public README, LICENSE, v0.7.11 Release, and the specs and rea output above. It did not install or run DESIGN:OS Studio, did not rerun rea, and did not independently reproduce .fig compatibility or editor behaviour. The star count is a snapshot only, not evidence of those capabilities.

Snapshot 2026-11-10: GitHub shows 87 stars; release v0.7.11.
License: PolyForm Shield 1.0.0 (source-available, not open source). README-documented issue #834 remains open.
REA evidence is in public specs and checked-in CLI output; the product README does not credit REA. Some failed rea invocations are recorded as-is.

## Sources

- [Spec E1-4: morluto/rea 6.7.0 method note (commit df14c593e86edcc039adc2c67067bf8db64e9e84)](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/docs/specs/v0.6/E1-4-styles-hold-variable-aliases.md)
- [Checked-in rea CLI evidence: inspect-macho and analyze-javascript-application](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/plans/reports/agy-1277-shadow-knockout-evidence/step1-figma-re.log)
- [Project README (commit df14c593e86edcc039adc2c67067bf8db64e9e84)](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/README.md)
- [LICENSE: PolyForm Shield 1.0.0](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/LICENSE)
- [v0.7.11 Release](https://github.com/jangtrinh/design-os-studio/releases/tag/v0.7.11)

[中文](../design-os-studio-fig-format.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
