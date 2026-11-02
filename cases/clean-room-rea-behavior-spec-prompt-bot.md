# Clean Room：PixelRainbow以REA输出行为规格与隔离会话重建提示的bot

分类：应用与客户端 · REA
记录日期：2026-11-03
阶段：相关项目

2026年10月31日05:58:58（北京时间），PixelRainbow（@PixelRainbowNFT）在Reverse Lab介绍中另列REA版Clean Room bot；06:10:51长帖说明把原系统研究和新实现分开，以减少同一上下文携带原始表达。用户提供有权研究的目标，bot访谈后驱动morluto/rea追踪操作到结果，将主张标为Observation／Inference／Unknown并引用Evidence，形成行为SPEC.md；怀疑式裁判检查证据和污染，人工批准后再访谈平台、范围、差异与验收，输出带XML标签、号称做过变异测试的PROMPT.md，交给未看原目标的新Opus 5.5会话。它是研究／交接项目，不是某个应用已经重建。

10月31日08:49:14作者曾称即使Ultra也一直缺Grokbot token。没有计数、账单或日志，不能推出完成过交接、具体成本或所有订阅不可用。这是较早使用约束，不用后续功能宣传默认为已解决。

11月3日00:41:01，同作者介绍REA版Grokbot模板四项更新：Swarm让控制器按函数派工、统一结构名、对置信度低于6的结果二次检查，并按函数组记支出；混淆skill先定预算、剔除垃圾代码、按证据命名技术，未解多层标unknown；SPEC依次列Feature summary、Architecture、Data Model、Public API、File Formats、Rules、Test Cases、Open unknowns。裁判退回缺正常／边界／错误测试的规则，但作者明确模板裁判已更新、live bot仍是旧措辞，不能当部署一致。

默认构建提示新增50输入对照（30正常、10边界、10错误）及三个故意破坏的构建，关键和行为用例要求100%；访谈仍可选mutants-only取消50输入。这些是交给后续建造者的要求，不代表Clean Room自己开始运行构建，也不是50项或变异测试已经通过。新帖另链接Ghidra／leanrea版，属于另一模板，不把其功能混入REA版；新帖未重述Clean Room名称，按同作者的REA／SPEC／裁判／访谈交接工作流补证，未独立核验模板链接身份。

旧帖明确静态优先、启动或接触在线目标需逐次许可。未取得bot配置、完整SPEC、原始测试日志、隔离验证或行为等价记录；“one-shot”“proven contract”仍是作者宣传，不保证法律安全或正确重建。补取原帖确认署名与文字，未打开bot、安装REA、执行目标或发起重建。

较早三帖快照分别1赞／151浏览／0转发、1赞／227浏览／0转发、0赞／194浏览／0转发；11月3日候选2赞／319浏览／0转发。
置信度6、50输入、30／10／10、三个破坏构建及100%是模板规则，不是实测通过数。

## 来源

- [PixelRainbow在Reverse Lab帖中首次另列Clean Room，2026-10-31 05:58:58](https://x.com/i/status/2116288779254198577)
- [PixelRainbow的Clean Room规格与提示交接长帖，2026-10-31 06:10:51](https://x.com/i/status/2116291769230926128)
- [作者补充Ultra订阅仍缺Grokbot token的限制，2026-10-31 08:49](https://x.com/i/status/2116331630461620246)
- [同作者REA模板四项更新及live bot差异，2026-11-03](https://x.com/i/status/2117295928742658556)

[English](en/clean-room-rea-behavior-spec-prompt-bot.md) | [返回目录](../README.zh-CN.md)
