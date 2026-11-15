# WebsiteBench：从浏览器探索重建全栈网站，以隐藏功能测试和视觉对照检验

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：分析测试

2026年11月15日06:02:13（北京时间），Johnnysama（@JohnnyS03832498）介绍WebsiteBench：Agent只从浏览器探索生产级网站，重建尽量匹配外观和行为的全栈实现，不只临摹截图。补查定位TIGER-AI-Lab/WebsiteBench并阅读固定README，提交3868d82d137f4ff8f5b2bd858ed8c279da3aeda1日期为2026年11月10日06:47:19 UTC，早于窗口；这是项目方法补证，不是新候选或本合集运行成绩。

文档列70个网站、46916个隐藏测试，每任务302至2016个。一个测试须功能检查通过且每个视觉检查点的归一化SSIM达0.99才通过；任务reward为通过的测试比例，不是整个网站已被完整克隆的概率。文档给Harbor执行和参考解检查方式，但本合集未安装依赖、下载任务或执行评测。

候选称Opus5.5隐藏测试通过26%、请求层面71%，Amazon56.8%、LeetCode最高74.2%；DeepSeek V4.1 Flash为13.5%、每任务4.6美元，Opus为305美元。这些是评论者的快照，所读README没有模型排行榜、请求指标定义、成本核算或单站结果，故未独立确认，不能混合两种百分比、推算完整复制率或可比成本降幅。没有REA实用证据；未加额外harness只是评论者推测。

README称评测代码、任务定义和verifier为Apache-2.0；参考站点的第三方内容仍归原权利人，仅供非商业研究。未检查全部许可或参考实现，不意味着获得生产站点内容再分发权。按有公开评测方法的AI辅助黑箱功能重建案例收录，结果仍归项目或评论者，不是独立复现。

封存候选2赞、72浏览、0转发、1回复；26%／71%属不同指标，模型版本、成本与单站成绩未据原始结果复核。

## 来源

- [Johnnysama介绍WebsiteBench及模型分数／成本，2026-11-15 06:02:13北京时间](https://x.com/i/status/2121725416557908217)
- [窗口前固定README：任务规模、SSIM评分与许可，提交2026-11-10 06:47:19 UTC](https://github.com/TIGER-AI-Lab/WebsiteBench/blob/3868d82d137f4ff8f5b2bd858ed8c279da3aeda1/README.md)

[English](en/websitebench-browser-only-fullstack-reconstruction-benchmark.md) | [返回目录](../README.zh-CN.md)
