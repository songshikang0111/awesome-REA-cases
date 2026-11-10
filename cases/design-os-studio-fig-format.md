# DESIGN:OS Studio：用 REA 逆向 Figma .fig 并重实现编辑器的桌面工作室

分类：应用与客户端 · REA
记录日期：2026-11-10

DESIGN:OS Studio 是 Jang Trịnh（jangtrinh）发布的本地桌面设计工作室，公开仓库为 https://github.com/jangtrinh/design-os-studio。审阅提交 df14c593e86edcc039adc2c67067bf8db64e9e84 的 README（发布版本 v0.7.11）写明：可读取 Figma 的 .fig 容器（fig-kiwi，DEFLATE 或 Zstd），写出容器版本 106，并在本地重实现编辑器行为。附带通过 stdio 提供的 designos-mcp 服务器，README 生成的工具表列出 39 个工具，可从选定图层生成 CSS、Tailwind、React、SwiftUI、UIKit、Compose、Android XML 或 HTML。仓库同时说明 macOS CI 上有 6000 余项测试。

同一提交中的公开规格将逆向 Figma 字段的规则写为使用 `rea`（morluto/rea）。E1-4（2026-10-18）记载：`rea`（morluto/rea 6.7.0，`npx -y rea-agents`）对提取出的编辑器 JavaScript 运行了 analyze-javascript-application（证据 `ev_2624766…`）；wasm 路径当时不可用（未安装 WABT 与 Ghidra），因此用约 40 行的本地 kiwi decodeBinarySchema 读取器解码 schema。plans/261017-figma-parity-wave-ab/rea-findings.md 写明方法包含静态 `rg` 与 REA。plans/reports 中还存有已完成的 rea inspect-macho 与 analyze-javascript-application 输出，以及部分失败调用。产品 README 没有提及 REA。维护者 Jang Trịnh 于 2026-11-10 确认此项 Figma 工作使用了 REA。

许可为 PolyForm Shield 1.0.0，属于源码可用，不是开源协议。README 记载的已知问题 #834 仍未关闭：保存 .fig 时编号列表格式会丢失，实例上继承或变量绑定的填色会被写成固定值。

本合集查阅了公开 README、LICENSE、v0.7.11 Release 以及上述规格与 rea 输出，未安装或运行 DESIGN:OS Studio，未重跑 rea，也未对 .fig 兼容性或编辑器行为做独立复现。星标数量仅作快照，不作为功能证据。

快照 2026-11-10：GitHub 显示 87 star；发布版本 v0.7.11。
许可：PolyForm Shield 1.0.0（源码可用，非开源）。README 记载已知问题 #834 仍开放。
REA 证据在公开规格与入库 CLI 输出中；产品 README 未署明 REA。部分 rea 调用失败已如实记录。

## 来源

- [规格 E1-4：morluto/rea 6.7.0 方法说明（提交 df14c593e86edcc039adc2c67067bf8db64e9e84）](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/docs/specs/v0.6/E1-4-styles-hold-variable-aliases.md)
- [入库的 rea CLI 证据：inspect-macho 与 analyze-javascript-application](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/plans/reports/agy-1277-shadow-knockout-evidence/step1-figma-re.log)
- [项目 README（提交 df14c593e86edcc039adc2c67067bf8db64e9e84）](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/README.md)
- [LICENSE：PolyForm Shield 1.0.0](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/LICENSE)
- [v0.7.11 Release](https://github.com/jangtrinh/design-os-studio/releases/tag/v0.7.11)

[English](en/design-os-studio-fig-format.md) | [返回目录](../README.zh-CN.md)
