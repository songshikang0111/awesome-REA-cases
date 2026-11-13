# Fable故事动画拆解：Ganesh用Claude与REA观察一轮生成，训练机制仍是推测

分类：应用与客户端 · REA
记录日期：2026-11-13
阶段：分析测试

2026年11月13日16:36:03（北京时间），Ganesh Iyer（@ganeshiyer316）称当周用Claude Code与REA拆解两款故事动画应用，原因是想把七岁女儿写的故事做成短片，现有工具昂贵且不完全合用。他在每款应用各做一个故事，让REA观察请求与响应、只保留字段名，再由Claude按自写product-teardown技能整理报告。两款目标分别保留记录；此条对应回复明确提到的Fable动画产品，不是把同名模型Fable当成目标。没有报告完成自用替代品。

16:55:14，Harrison追问每角色训练模型的依据；17:05:36 Ganesh承认没有看到训练，角色已建好，只是在每个故事的角色数据里看到trigger word与finished training标记，据此猜测定制图像模型。字段是作者声称观察到的线索，训练行为、模型供应商与服务端流水线都未直接观察，不能把“Seen”标签扩大成整套架构100%确认。这两条补查回复不是额外候选。

补读公开技能README与SKILL，固定仓库版本81dd09b019a342a06906e44e8245aaf89e915f29提交于同日16:58:10，晚于主帖，作为实现说明而非原始抓取证据。文档要求用户操作合法账号、只观察、不重放请求、不保存正文／头／cookies／token或源码；输出Seen／Best guess与未知项。README只称macOS上Claude Code测过，Linux、Windows和Codex未测；页面跳转与提前建立的连接会造成缺口。本合集只读文档与作者回复，未审原始流量、运行技能、登录产品或复现推断。

主候选快照3赞、156浏览、0转发、4回复；这是两目标共用的帖子，不分别累加热度。

## 来源

- [候选：Ganesh的两款故事动画应用拆解，2026-11-13 16:36:03北京时间](https://x.com/i/status/2121160150278926639)
- [补充追问：Fable角色训练依据，16:55:14](https://x.com/i/status/2121164975842685060)
- [补充作者更正：未看到训练，17:05:36](https://x.com/i/status/2121167585735737473)
- [固定product-teardown README，版本提交于2026-11-13 16:58:10北京时间](https://github.com/ganeshiyer316/claude-skills/blob/81dd09b019a342a06906e44e8245aaf89e915f29/skills/product-teardown/README.md)
- [固定SKILL：观察边界、字段与推断标签](https://github.com/ganeshiyer316/claude-skills/blob/81dd09b019a342a06906e44e8245aaf89e915f29/skills/product-teardown/SKILL.md)

[English](en/ganesh-fable-animation-rea-traffic-teardown.md) | [返回目录](../README.zh-CN.md)
