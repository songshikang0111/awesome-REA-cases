# Meta Hyperscape：Stefano Rivera用Claude研究渲染器，卡在60万splat

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-10
阶段：待验证

2026年11月10日16:54:03（北京时间），Stefano Rivera（@easyldur）在讨论中说自己最近逆向了Meta Hyperscape，并补充实际工作由Claude完成。他认为这是性能最好的高斯splat渲染器，但无论怎么做总量都无法超过600k，于是询问对方使用什么方案。高斯splat是一种以大量三维高斯元素表示场景的渲染方法；本条目标是理解并尝试扩大该渲染器的场景容量。

补取原帖确认署名与文字，没有Hyperscape版本、被分析文件、Claude模型、方法、代码、硬件、显存、帧率或600k限制的错误信息。不能判定它是硬编码上限、资源不足或实验配置问题，也不能把作者最优性能评价当独立排名。600k按总splat数量理解，不改写成每秒或模型参数量；未说明成功恢复源码或突破限制。

按带有失败边界的作者研究报告收录，REA未说明。本合集没有运行渲染器或取得场景，不证明Claude分析准确或Meta产品固有上限。

候选封存1赞、37浏览、0转发；600k为作者实验总量，不是基准测试。

## 来源

- [Stefano Rivera的Claude／Hyperscape与600k瓶颈自述，2026-11-10 16:54:03北京时间](https://x.com/i/status/2120077516803326162)

[English](en/easyldur-meta-hyperscape-claude-splat-limit.md) | [返回目录](../README.zh-CN.md)
