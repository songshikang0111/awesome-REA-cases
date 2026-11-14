# DESIGN:OS Studio：REA研究Figma JS与.fig格式，公开Rust本地设计工具

分类：应用与客户端 · REA
记录日期：2026-11-11
阶段：进行中

2026年11月11日16:30:17（北京时间），yibie（@yibie）的每日清单介绍DESIGN:OS Studio，称它用REA研究Figma桌面JavaScript与.fig v106的kiwi schema，并重新实现桌面端。目标是拥有本地设计文件与可供Agent操作的原生设计工具，而不是恢复Figma全部源码。该帖另含MK64 PS3，是不同目标，单独收录。

补查作者在yibie/awesome-rea的PR #7及固定规格E1-4。PR于11月10日22:51:19北京时间提出、11月11日13:35:36合并，均早于窗口；规格固定于11月10日21:44:10的df14c593e86edcc039adc2c67067bf8db64e9e84提交，内部研究注明10月18日，并有10月19日修订，不能把这些原始工作日期当本轮实验。规格明确REA6.7.0在提取的Figma缓存JS上运行analyze-javascript-application；本机没有WABT和Ghidra，wasm分析路线不可用，改以40行kiwi schema读器解析wasm数据段。作者报告653定义及一个v106、56625节点.fig样本，对照样式变量绑定；区分观察事实与fontStyle字符串绑定推断。维护者 Jang Trịnh 在本合集 PR #4 中确认，这项 Figma 工作使用了 REA。其提供的公开日志记录了已完成的 inspect-macho 和 analyze-javascript-application 调用。未审阅完整 REA 原始报告或独立复算字段，规格中的事实仍为项目研究记录，不能称REA独自完成所有解析。

另读固定提交1cc765bca900e187431d079f892f402cbaa200c7的README相关章节，提交于11月11日19:45:34北京时间，晚于候选。文档描述Rust／wgpu与tiny-skia、本地.fig读写、输出container v106、运行用户自己的Agent CLI的面板和stdio MCP。超过6000项macOS CI测试与大文件数据是项目自报，未审CI日志、源码实现或复跑。

README写明没有实时多人云协作或企业云管理；已知.fig保存会丢编号列表格式，并把实例的继承／变量绑定paint写成固定值。发布说明与旧问题列表有局部不一致，不能据新增修复段落宣布所有保存问题已解决。v0.7.11 Windows CI失败，Windows测试为advisory，发布前以macOS验证为主，Linux包构建不等于试玩确认。Agent各自计费，不因Studio不用额外API key而免费。当前为PolyForm Shield 1.0.0 source-available，不泛称OSI开源；文档称旧版至v0.5.0保留MIT或Apache许可。未运行目标、安装依赖或比较Figma输出，不认定全功能等价。

整条清单封存2赞、249浏览、0转发，不是单个项目热度；PR状态为本次读取快照，不作为完整功能验证。

## 来源

- [yibie清单：Figma JS、kiwi v106与REA研究转述，2026-11-11 16:30:17北京时间](https://x.com/i/status/2120433924434452690)
- [补充项目README功能与限制，固定2026-11-11 19:45:34北京时间提交](https://github.com/jangtrinh/design-os-studio/blob/1cc765bca900e187431d079f892f402cbaa200c7/README.md)
- [补充原始规格E1-4：10月18至19日REA研究，固定11月10日窗口前提交](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/docs/specs/v0.6/E1-4-styles-hold-variable-aliases.md)
- [补充作者提交说明PR #7，2026-11-10提出、11-11窗口前合并](https://github.com/yibie/awesome-rea/pull/7)
- [维护者 Jang Trịnh 的提交与 REA 使用确认（本合集 PR #4）](https://github.com/songshikang0111/awesome-REA-cases/pull/4)
- [项目公开的 REA 命令行记录（固定提交）](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/plans/reports/agy-1277-shadow-knockout-evidence/step1-figma-re.log)
- [项目许可证 PolyForm Shield 1.0.0（固定提交）](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/LICENSE)
- [项目发布说明 v0.7.11](https://github.com/jangtrinh/design-os-studio/releases/tag/v0.7.11)

[English](en/design-os-studio-figma-js-kiwi-rebuild.md) | [返回目录](../README.zh-CN.md)
