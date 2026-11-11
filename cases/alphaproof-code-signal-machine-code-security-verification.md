# AlphaProof Code与Signal：团队报告一个月证明生产机器码的关键安全属性

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-11
阶段：相关项目

2026年11月10日20:13:07（北京时间）的团队宣布帖称，Google DeepMind以AlphaProof Code证明Signal通信协议底层生产机器码的关键安全属性。用途是检查协议落地到设备运行代码时的安全性质，而不只验证简化设计模型；因此作为AI辅助二进制分析相关项目收录，不称传统反编译或克隆Signal。

原帖把AlphaProof Code描述为运行在含Gemini Carbon等LLM上的agentic形式验证框架，称类似研究可能需要团队数十年累计工作，而本次在一个月内完成，并宣布开放形式规格及验证产物。作者将“首个在此深度验证广泛部署协议生产代码”的地位作为团队主张，本合集未作历史优先权核验。帖中列Swarat Chaudhuri、Andrew Ferraiuolo、Anton Kovsharov、Tej Chajed、Sam Schlesinger、Karn Seth、Jonathan Katz与Charles Sutton等成员，并感谢Signal合作。

11月11日15:14:13，青雲（@echo_vic）转述阅读结果，称目标为libsignal v0.105.4编译的AArch64二进制，约14万条指令；五人四周、约650万行Lean证明。同一机器运行40至80个Agent，一轮24至72小时；证明由Carbon写，规格由Carbon与Claude Opus 5.5共同起草，再由人批准。帖子称重新植入两项历史bug后，系统证明修改二进制违反定理，以此检查规格是否足够严格；真正需信任的规格与机器语义约2.6万行。以上是具名读者的详细转述，本合集补查仅确认其署名与完整文字，没有读取原博客、版本构建、规格、证明仓库或检查器记录。

早期转述还出现三百余万行等不同计数，不把它们和650万行合并成确定值；行数、并发数及四周也不是准确率或独立工时测量。帖中seL4二十人年的比较跨目标、规格与工程条件，不能据此计算通用加速比。不信任编译器并不等于没有信任基础，规格、机器语义与证明检查器仍需审查。没有独立运行检查器，也未核对威胁模型、确切组件与假设；关键属性不等于所有Signal代码、配置和攻击面无漏洞。REA未提及。

旧团队帖封存2919赞、155181浏览、352转发；传播不是形式规格或证明检查结果的独立核验。
青雲候选封存0赞、18浏览、0转发；版本、规模和并发数为其转述，未审证明库。

## 来源

- [DeepMind团队宣布AlphaProof Code验证Signal生产机器码，2026-11-10 20:13:07北京时间](https://x.com/i/status/2120127611137634376)
- [青雲转述libsignal版本、Agent运行、Lean规格与历史bug反例，2026-11-11 15:14:13北京时间](https://x.com/i/status/2120414781471596548)

[English](en/alphaproof-code-signal-machine-code-security-verification.md) | [返回目录](../README.zh-CN.md)
