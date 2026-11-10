# DESIGN:OS Studio: an independent desktop studio that reads and writes Figma .fig files and reimplements the editor

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-10

DESIGN:OS Studio is a local desktop design studio published by Jang Trịnh (jangtrinh). The public repository is https://github.com/jangtrinh/design-os-studio. The README at reviewed commit df14c593e86edcc039adc2c67067bf8db64e9e84 (release v0.7.11) states that it reads Figma .fig containers (fig-kiwi, DEFLATE or Zstd), writes container version 106, and reimplements editor behaviour locally. A bundled designos-mcp server serves tools over stdio. The README's generated tool table lists 39 tools, and selected layers can be turned into CSS, Tailwind, React, SwiftUI, UIKit, Compose, Android XML or HTML. The repository also describes more than 6,000 tests on macOS CI.

The license is PolyForm Shield 1.0.0: source-available, not an open-source license. A known issue documented in the README, #834, remains open: saving a .fig file drops numbered-list formatting and writes inherited or variable-bound paints on instances as fixed values. The repository does not state use of morluto/rea, and it does not say whether the format and editor work was done by hand or with AI assistance, so REA use remains unknown.

This collection reviewed the public README, LICENSE and v0.7.11 Release page. It did not install or run DESIGN:OS Studio, and it did not independently reproduce .fig compatibility or editor behaviour. The star count is a snapshot only, not evidence of those capabilities.

Snapshot 2026-11-10: GitHub shows 87 stars; release v0.7.11.
License: PolyForm Shield 1.0.0 (source-available, not open source). README-documented issue #834 remains open.

## Sources

- [Project README (commit df14c593e86edcc039adc2c67067bf8db64e9e84)](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/README.md)
- [LICENSE: PolyForm Shield 1.0.0](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/LICENSE)
- [v0.7.11 Release](https://github.com/jangtrinh/design-os-studio/releases/tag/v0.7.11)

[中文](../design-os-studio-fig-format.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
