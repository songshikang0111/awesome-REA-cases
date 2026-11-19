# NotTheInstagram：FLEX给Codex指路，用REA给无限刷加阻力

分类：应用与客户端 · REA
记录日期：2026-11-20
阶段：待验证

2026年11月20日01:01（北京时间），lifcc（@mylifcc）介绍NotTheInstagram并附原文与仓库线索。补读Kunal Kamble于11月15日发表的原文与项目文档：他不想删除Instagram、失去朋友私信，而要保留搜索等有用功能，给无限刷增加阻力。补充材料早于本轮严格窗口，不计新候选。

作者用Codex，经REA连接Hopper研究约400MB可执行文件。模型起初猜类名、找不到Explore网格；人用FLEX检查屏幕视图树，给模型类名与截图，再定位IGExploreGridViewController的viewWillLayoutSubviews并编写Objective-C hook。AGENTS.md记录协作约束，agents目录保存研究与测试状态；原文关键地图是FLEX视图树，不是转述所称一次Runtime Dump后写好的完整架构。重签名后Meta共享存储不可用还导致登录失败和崩溃，作者报告用适配层处理。

项目报告每3条信息流等待8、11、14秒，后续维持14秒；Reels入口等2分钟，每条播放前从3秒起递增0.5秒；私信视频不连播下一条，另显示使用时长。大部分工作一个下午完成是作者估量，不是完整项目工时。README所列测试环境为Instagram455.0.0、iPhone15、iOS27.0.1。

静态补读11月15日提交206eac2的README、RuntimeHooks.h与Explore笔记，可见替换前检查方法返回值、参数数量和类型。笔记明确静态元数据不是运行轨迹，搜索、旋转、无障碍等细项未全获实机确认；隐藏网格也可能继续请求数据。未构建、取得IPA或实机复现，不保证所有更新兼容；自备合法目标，修改客户端有平台规则与账号风险，保持unverified。

候选封存3赞、628浏览、0转发、1回复；来源回复0赞、171浏览，非项目总热度。

## 来源

- [lifcc介绍NotTheInstagram，2026-11-20](https://x.com/i/status/2123461551197720607)
- [同串文章与源码线索](https://x.com/i/status/2123461552271446033)
- [补充：Kunal原文，2026-11-15发表](https://rationalkunal.in/writing/make-instagram-boring-with-an-ai-agent/)
- [补充：固定11月15日提交的README](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/README.md)
- [补充：方法签名检查实现，静态阅读](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/NotTheInstagramFrameworkCode/NotTheInstagramFrameworkCode/Runtime/RuntimeHooks.h)
- [补充：Explore笔记及待实机检查](https://github.com/rational-kunal/NotTheInstagram/blob/206eac2ed1175a254df7db58f75ac7bcac127b3b/agents/search-investigation/explore-grid-notes.md)

[English](en/nottheinstagram-rea-codex-flex-friction-hooks.md) | [返回目录](../README.zh-CN.md)
