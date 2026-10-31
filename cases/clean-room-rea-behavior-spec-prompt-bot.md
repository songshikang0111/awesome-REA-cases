# Clean Room：PixelRainbow以REA输出行为规格与隔离会话重建提示的bot

分类：应用与客户端 · REA
记录日期：2026-10-31
阶段：相关项目

2026年10月31日05:58:58（北京时间），PixelRainbow（@PixelRainbowNFT）在Reverse Lab介绍中另列REA版Clean Room bot；06:10:51的独立长帖进一步说明目标是把研究原系统和写新实现分开，减少同一模型上下文携带原始表达的风险。它是辅助研究与交接的相关项目，不是已交付某个闭源应用的重建。

作者称用户提供有权研究的网站、应用、APK、二进制、抓包、文件或仓库，bot先访谈，再驱动morluto的REA追踪从操作到结果的真实路径，将主张标为Observation／Inference／Unknown并引用Evidence，输出只写行为的SPEC.md。怀疑式裁判逐项核对证据，对薄弱规则要求继续调查，做污染检查，等待用户批准。之后访谈重建意图、范围、差异、平台、技术栈、约束、验收与测试，形成带XML标签、号称做过变异测试的PROMPT.md，交给没看过原目标的新Opus 5.5会话。

08:49:14补充帖称，自己另做了使用REA的Clean Room bot，但即使有Ultra订阅，仍一直没有足够Grokbot token来使用它。这是作者的实际使用约束自述，没有token计数、账单或运行日志，不能推出完成过一次完整交接、具体成本或所有订阅都不可用。

作者明确Clean Room不交付应用、不运行构建；静态优先，启动或接触在线目标需逐次许可。没有bot配置、完整示例SPEC、变异测试日志、跨会话隔离验证或行为等价结果；“proven contract”仅为宣传措辞，不是法律无风险、无版权污染或正确重建保证。补查确认作者与正文；未打开bot、安装REA、执行目标或发起重建。

较早两帖快照分别1赞／151浏览／0转发与1赞／227浏览／0转发；本窗口补充为0赞／194浏览／0转发；未独立验收bot。

## 来源

- [PixelRainbow在Reverse Lab帖中首次另列Clean Room，2026-10-31 05:58:58](https://x.com/i/status/2116288779254198577)
- [PixelRainbow的Clean Room规格与提示交接长帖，2026-10-31 06:10:51](https://x.com/i/status/2116291769230926128)
- [作者补充Ultra订阅仍缺Grokbot token的限制，2026-10-31 08:49](https://x.com/i/status/2116331630461620246)

[English](en/clean-room-rea-behavior-spec-prompt-bot.md) | [返回目录](../README.zh-CN.md)
