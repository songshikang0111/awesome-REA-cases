# Reverse Lab：PixelRainbow以leanrea分诊与路由减少先全面反编译的工作流

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-31
阶段：相关项目

2026年10月31日05:58:58（北京时间），PixelRainbow（@PixelRainbowNFT）介绍Reverse Lab bot。目标是避免Agent为一个小问题先反编译整个程序、耗尽上下文：先批量清点file、字符串、导入与受限切片，逐项标记SEEN／INFERRED／UNKNOWN；按目标类型路由到Asar切片、go version -m、jadx等；只有字符串与元数据无法回答时才升级反编译或GhidraMCP。

作者明确将CLI优先的分诊／路由方法归于@aicodeking的leanrea，Ghidra用于深入原生二进制的交叉引用、调用图与类型恢复。08:49:14补充帖明确这是Grokbot Template，GhidraMCP取自@lauriewired，并与Lean REA的CLI工具组合。这里新增封装环境与上游归属，不称作者发明这些工具；同帖另提REA版Clean Room，独立记录其token限制。

帖子说在问题有证据时停止而非追求理解完整二进制，并要求只研究有权检查的目标。但没有实际样本、完整输出、提示配置、源码、耗时或token对照，不能据此证实比REA便宜多少、准确率更高或权限边界实际有效。补查两帖确认署名与文字；没有打开bot、安装工具或执行目标。

较早快照1赞、151浏览、0转发；补充候选0赞、194浏览、0转发；没有成本或效果基准。

## 来源

- [PixelRainbow介绍Reverse Lab与leanrea上游，2026-10-31 05:58:58](https://x.com/i/status/2116288779254198577)
- [PixelRainbow补充Grokbot模板与lauriewired的GhidraMCP归属，2026-10-31 08:49](https://x.com/i/status/2116331630461620246)

[English](en/reverse-lab-leanrea-triage-bot.md) | [返回目录](../README.zh-CN.md)
