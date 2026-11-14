# TinyTurla-NG静态重建：可编译C++与92.8%结构相似，不是运行验证

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-10
阶段：分析测试

2026年11月10日21:36:11（北京时间）的候选转述Intezer用AI重建Slack、Finder及Turla，并将后者描述为working replicant。补读Nicole（@NicoleFishi19）同日23:54的团队串后，目标可具体到TinyTurla-NG后门；本条仅记录防守研究中的静态理解与代码重建，不提供部署或攻击步骤。

23:54:12的帖明确说仅从静态分析得到可编译C++，从未执行，结构相似度92.8%；GPT-5.6运行工作流，Kimi K3审查，Binary Ninja作为ground truth。总述也说明从编译应用开始，结果依赖打包而非一键恢复。这些补充帖晚于候选，修正对working的保守解释：可编译和结构指标不证明后门实际行为、通信或任何恶意能力已成功复现。

未取得样本哈希、版本、结构相似度算法与分母、逐函数对照、编译日志、复核记录或公开代码；Binary Ninja对照是项目所述，不是本合集独立验证。候选链接报道正文未读到。REA未提及，本合集未下载、编译或执行恶意样本，也不推断其来源、部署环境或实际攻击效果。

候选封存0赞、112浏览、0转发；92.8%不是字节匹配、行为等价或攻击成功率。

## 来源

- [候选：Intezer研究与working Turla replicant转述，2026-11-10 21:36:11北京时间](https://x.com/i/status/2120148514973819118)
- [补充Nicole团队串总述：TinyTurla-NG目标，同日23:54:10](https://x.com/i/status/2120183240434872570)
- [补充Nicole：静态分析、可编译C++、92.8%与未执行边界，同日23:54:12](https://x.com/i/status/2120183247724273962)

[English](en/intezer-tinyturla-ng-static-cpp-reconstruction.md) | [返回目录](../README.zh-CN.md)
