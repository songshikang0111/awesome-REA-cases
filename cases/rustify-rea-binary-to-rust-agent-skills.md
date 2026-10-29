# Rustify：用REA证据、产品规格与分片验证组织二进制到Rust重建

分类：应用与客户端 · REA
记录日期：2026-10-29
阶段：进行中

2026年10月29日15:46:53（北京时间），Runchao Han（@runchao_han）介绍Rustify可通过Agent Skills用于Claude Code、Codex、Cursor和OpenCode，并依赖REA逆向。补读SebastianElvis/rustify固定提交1bbc4ba3506f558f448ffaa4372266f2bb89da96的README，提交时间2026-10-29T02:33:34Z，早于原候选窗口，只作项目背景。

工具不是单纯把反编译C逐行转Rust，而是要求从二进制和运行证据恢复产品行为、UX与架构，维护recovered/规格与证据、implementation/Rust仓库、verification/对照结果三类产物。八个技能覆盖准备、REA probe、产品/设计/架构发现、计划、分片实现与验证；台账把需求、证据、测试、组件、模块及缺口连接，目标变化应使过时结果失效。

README要求本地或云Agent都能访问REA、目标二进制、资源及兼容运行环境；桌面调查还需要GUI会话。完整产品等价是工作流目标与门槛，不是对所有目标完成的承诺。文档链接rustify-doom示例，称从stripped doomgeneric与Freedoom数据重建；又列base64、BLAKE3、HTTP、对话框、bzip2、Lua、SQLite、Ninja、Doom及macOS iconutil/textutil评估方向。本文只读README，没有读这些独立目标的验收记录，因此不宣称它们均已通过，也不把补充示例算作本轮独立候选。

同日23:37:44，Runchao在本窗口回复中补充：软件移植适合训练AI模型，REA可从原始二进制提取执行轨迹，再用trace validation客观测量保真度。它提出了比泛称等价更具体的验证方向，但未附目标、轨迹、误差或通过记录，不意味着Rustify已经实现或完成所有这种测试。新候选快照1赞、10浏览、0转发；不覆盖较早传播快照。

公开项目声明Apache-2.0，部分上游测试保留各自许可；重建目标仍需合法分析权。本合集未安装技能、配置REA、运行二进制、编译Rust或复测等价。按有公开工作流、仍需目标验证的进行中工具项目收录。

较早候选快照0赞、16浏览、0转发；新回复1赞、10浏览、0转发；仓库README为较早补证。
全产品重建与等价为目标；轨迹验证是新提出的方向，未独立运行，不将示例或评估目录当通过证明。

## 来源

- [Runchao Han介绍Rustify的跨Agent支持与REA依赖，2026-10-29](https://x.com/i/status/2115711957554851944)
- [补充：Rustify固定提交README，10月29日02:33:34Z，早于原候选窗口](https://github.com/SebastianElvis/rustify/blob/1bbc4ba3506f558f448ffaa4372266f2bb89da96/README.md)
- [Runchao补充执行轨迹与保真度验证方向，2026-10-29 23:37:44](https://x.com/i/status/2115830452510720014)

[English](en/rustify-rea-binary-to-rust-agent-skills.md) | [返回目录](../README.zh-CN.md)
