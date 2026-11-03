# REA Launcher SDK：Fabio Makita把旧赛车互通经验提炼为Agent启动器框架

分类：游戏与游戏保存 · REA
记录日期：2026-11-03
阶段：进行中

2026年11月3日09:30（北京时间），Fabio Makita（@AkitaOnRails）发布REA Launcher SDK，称在为Colin McRae系列、OutRun、Sega Rally、Screamer等做启动器后，把共同部分提炼出来，供编程harness创建新游戏启动器。他说应能完成约90%的工作，是作者预期，不是游戏覆盖率或统一验收成绩。

补读akitaonrails/rea-launcher-sdk提交050d3b3ad4b4840efab744fd65b15d17e60787f3的README，提交时间为11月3日09:54北京时间，晚于候选但仍在窗口，仅作补充项目材料。文档明确由Claude Code、Codex、opencode、Cursor等Agent研究、逆向和写代码，人提供游戏与决策；先研究社区修复，再在研究发现、选项和实机验证处让人审阅。共享部分包括Rust核心、Windows辅助与UI、Linux/Wine脚本、AppImage打包及复用CI。

目标是让玩家自己的旧PC游戏在现代Windows/Linux运行并可配置，不是重建完整游戏或分发资产。项目规则称原游戏目录只读，变化落在私有运行副本，组件固定URL并校验SHA256；行为改变必须逐游戏验证后才能默认启用。README列有headless、Wine和Rust检查命令，不等于本合集已执行；未安装依赖、构建启动器或运行游戏。MIT或Apache-2.0双许可为文档声明，不能外推到游戏与第三方组件。

候选快照25赞、1558浏览、2转发；90%是作者估计，未运行项目测试。

## 来源

- [Fabio Makita的REA Launcher SDK发布，2026-11-03](https://x.com/i/status/2117429251741741227)
- [补充SDK固定README，提交2026-11-03 09:54北京时间](https://github.com/akitaonrails/rea-launcher-sdk/blob/050d3b3ad4b4840efab744fd65b15d17e60787f3/README.md)

[English](en/makita-rea-launcher-sdk-retro-games.md) | [返回目录](../README.zh-CN.md)
