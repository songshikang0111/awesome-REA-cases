# Instinct记忆黑盒拆解：Awake转述Git、Markdown、grep及隔夜抽取

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-05
阶段：待验证

2026年11月5日19:56:03（北京时间），Awake｜AI拆解（@hqluo11）以问答介绍Instinct记忆，归因Dhravya Shah黑盒逆向，明确未见源码、部分为推断。目标是理解AI Agent记忆的存储、检索与注入，而不是恢复模型权重；所选文本称Instinct，不擅自把它改名成Claude Code，也不因研究者相同合并两个目标。

帖子描述Git管理分层Markdown，YAML头含id／type／aliases，以[[id]]链接；分类包括人物组织、事实偏好决策、通信、时间线与工作流。主Agent以只读和grep检索，开场注入profile、一页纸、compaction与todo，不够再查工具；抽取约24小时异步进行。声称没有向量库、别名影响命中，并用pasta与Italian noodles作可能漏检的例子。上述均是转述机制与示例，非本合集确认的实现和测量。

作者认为Git利于历史与审计，但写入成本、遗忘、近因／过期／冲突治理仍有不足；这是评论，不是量化缺陷验证。没有原始文章全文、产品版本、提示词、记忆文件、观察轨迹或实验；未确认AI参与逆向，REA未知。保留AI产品黑盒行为研究的未核验二手报告，未访问任何私人记忆、执行检索或运行代码。

封存候选0赞、6浏览、0转发；机构实现与无向量库说法均未独立验证。

## 来源

- [Awake的Instinct记忆问答与黑盒推断声明，2026-11-05 19:56:03](https://x.com/i/status/2118311379853783547)

[English](en/instinct-memory-git-markdown-grep-blackbox-secondary-report.md) | [返回目录](../README.zh-CN.md)
