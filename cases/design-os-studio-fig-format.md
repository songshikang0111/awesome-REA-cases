# DESIGN:OS Studio：独立读写 Figma .fig 并重实现编辑器的桌面工作室

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-10

DESIGN:OS Studio 是 Jang Trịnh（jangtrinh）发布的本地桌面设计工作室，公开仓库为 https://github.com/jangtrinh/design-os-studio。审阅提交 df14c593e86edcc039adc2c67067bf8db64e9e84 的 README（发布版本 v0.7.11）写明：可读取 Figma 的 .fig 容器（fig-kiwi，DEFLATE 或 Zstd），写出容器版本 106，并在本地重实现编辑器行为。附带通过 stdio 提供的 designos-mcp 服务器，README 生成的工具表列出 39 个工具，可从选定图层生成 CSS、Tailwind、React、SwiftUI、UIKit、Compose、Android XML 或 HTML。仓库同时说明 macOS CI 上有 6000 余项测试。

许可为 PolyForm Shield 1.0.0，属于源码可用，不是开源协议。README 记载的已知问题 #834 仍未关闭：保存 .fig 时编号列表格式会丢失，实例上继承或变量绑定的填色会被写成固定值。仓库没有写明使用 morluto/rea，也没有说明这次格式与编辑器工作是手工完成还是由人工智能辅助，因此 REA 使用保持 unknown。

本合集查阅了公开 README、LICENSE 与 v0.7.11 Release 页面，未安装或运行 DESIGN:OS Studio，也未对 .fig 兼容性或编辑器行为做独立复现。星标数量仅作快照，不作为功能证据。

快照 2026-11-10：GitHub 显示 87 star；发布版本 v0.7.11。
许可：PolyForm Shield 1.0.0（源码可用，非开源）。README 记载已知问题 #834 仍开放。

## 来源

- [项目 README（提交 df14c593e86edcc039adc2c67067bf8db64e9e84）](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/README.md)
- [LICENSE：PolyForm Shield 1.0.0](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/LICENSE)
- [v0.7.11 Release](https://github.com/jangtrinh/design-os-studio/releases/tag/v0.7.11)

[English](en/design-os-studio-fig-format.md) | [返回目录](../README.zh-CN.md)
