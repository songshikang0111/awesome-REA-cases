# Hopper的DeepSeek二进制分析服务：去拒绝不等于逆向正确

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-05
阶段：相关项目

2026年11月5日06:51:15（北京时间），Hopper（@hopper_research）在Claude拒绝逆向的讨论下，称自己提供用于binary work的abliterated DeepSeek，即削弱模型拒答行为的改造版本，并给出HarmBench拒绝率从62.8%到0%的宣传数字。具体用途是为会中途拒答的二进制研究提供另一模型服务，不是已经完成某个目标的逆向。

拒绝率衡量的是是否回答，不能推出反编译正确、结构恢复完整或模型安全可靠。帖子没有DeepSeek版本、模型权重、修改方法、HarmBench样本与配置、评分规则、原始输出、代码或可核验服务文档，也未给任何二进制案例与对照。关于Claude普遍不再逆向的说法仅是该服务推广者的概括，不在这里当作厂商政策事实。

按相关AI逆向工具服务收录，status为related-project并不代表服务已验证。未调用服务、发送二进制或安装模型，REA未提；不把相邻引述中的可审计harness功能归给Hopper，也不把去拒绝宣传当作独立测试。

候选封存0赞、19浏览、0转发；补取热度未覆盖封存值，62.8%到0%未复核。

## 来源

- [候选及署名补查：Hopper的DeepSeek二进制服务与拒绝率，2026-11-05](https://x.com/i/status/2118113876516770042)

[English](en/hopper-abliterated-deepseek-binary-analysis-service-report.md) | [返回目录](../README.zh-CN.md)
