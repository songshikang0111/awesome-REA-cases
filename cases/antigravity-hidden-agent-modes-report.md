# Antigravity内部研究：隐藏模式、Gemini枚举分析与swarm白板调度报告

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：分析测试

2026年10月21日19:37（北京时间）的历史来源称Antigravity的jetski/language_server.exe藏有/owl、/battle、/benchmark、/compaction四种未公开多Agent模式，并推荐扩展Skill。其/battle被描述为两个subagent在隔离Git分支工作、critic选胜者合并，/benchmark用于测优化。该旧来源未给二进制版本、偏移、代码或命令记录，也未说明AI角色；四个名字是否内建可用、Skill是否调用隐藏实现仍未知，不能由新来源倒证。

10月28日13:57:26，Jerry Xiong（@Jerry_Galaxy）报告本地研究客户端2.27.0的156MB language_server，称看到Gemini4 Argon的High/Medium/Low，未见Carbon或4-Flash独立代号；发现MODEL_CUSTOM_VLLM、MODEL_CUSTOM_OPEN_ROUTER及Claude BYOK协议，又指出gemini-v4s-jarvis-sc、MODEL_GOOGLE_JARVIS_PROXY、Step_ClickBrowserPixel与鼠标、拖拽、键盘、DOM、滚动等浏览器动作，并列OrionFire、CosmicForge、RiftRunner及Thinking、InfinityBloom/InfinityJet。大小、代号和功能解释都是作者的静态分析报告，不当Google正式路线图。补查原帖确认署名和枚举截图附件；同日14:02:40作者也说最终以Google正式发布为准。

窗口外同日17:05:47，Jerry补充没有专业逆向工具：在Mac将安装包复制到独立工程目录，解压后直接让Gemini模型分析。这只补充当时候选的方法归因，不是另一候选或新实验；明确了AI角色，不推断REA参与。协议枚举至多表明客户端预留或包含字段，不证明服务可用、路由已上线、BYOK受支持或Jarvis完整可执行。没有二进制哈希、偏移、反编译文本、代码仓库、模型版本或运行验证，截图未独立核验；也不能以未见某代号证伪其他版本或服务端模型。

2026年11月15日03:06:41（北京时间），はるか（@HarukaKunori）建议逆向阅读agy的swarm实现，将它解释为白板共享信息、唤醒worker，并由少量特殊Agent兜底防死锁的调度。作者说白板默认视图隔离但不限制最终可见性，相当于外置上下文，认为在迭代／批量任务中可能比简单记忆或IRC加Handoff.md更抗压缩丢失信息。这里沿AI编程工具语境把agy视为Antigravity简称，但原帖未展开名称，不证明与旧2.27.0为同一版本或四个模式之一。

新帖提供具体架构解释，没有客户端版本、源码、偏移、逆向工具、实测任务、丢失率或死锁测试；未说明这次研究是否由AI执行，不能推成已证明性能胜出或彻底杜绝死锁。补取只确认作者、文字和图片附件，未解读图片。它是对同目标的补充观察，不倒证旧隐藏模式或枚举，也不与OpenCodex签名丢失项目混同。保留ID与历史URL，不提供启用指令，未取得或执行安装包、连接服务或独立复现，状态仍是analysis-test。

历史来源2026-10-21T19:37:00+08:00的隐藏模式仍未验证；新版本枚举不证明旧扩展行为。
10月28日候选快照3赞、523浏览、1转发；2.27.0、156MB及全部代号按作者报告，未运行目标。
10月28日17:05方法回复晚于当时窗口16:00 end，仅作方法补证；连续证据截止不因此推进。
11月15日候选封存4赞、216浏览、0转发、1回复；抗压缩和防死锁为架构解释／评价，没有对照测试；agy简称的对应保留不确定性。

## 来源

- [历史：Antigravity四个隐藏模式与扩展Skill转述，2026-10-21](https://x.com/i/status/2112870764991181226)
- [候选：Jerry的2.27.0 language_server枚举研究，2026-10-28](https://x.com/i/status/2115322026089205783)
- [同日14:02补充：作者称以Google正式发布为准](https://x.com/i/status/2115323343943729371)
- [窗口外同日17:05补证：Mac解包后用Gemini分析](https://x.com/i/status/2115369425616679197)
- [はるか的agy swarm白板／worker／防死锁调度解释，2026-11-15 03:06:41北京时间](https://x.com/i/status/2121681241212916029)

[English](en/antigravity-hidden-agent-modes-report.md) | [返回目录](../README.zh-CN.md)
