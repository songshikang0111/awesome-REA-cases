# Renfe CLI：研究网页API，让Agent查西班牙火车与延误

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-20
阶段：进行中

2026年11月20日03:49:13（北京时间），Luis González（@luisgonzaleznf）解释Renfe CLI核心是研究Renfe网页API，称@hugojm_正构建MCP，以便接入Claude、Instinct等Agent。Renfe是西班牙铁路运营商；目标是避免手工浏览复杂网站，查询车次、价格与延误并引导购票。没有说逆向本身由AI完成，按面向AI工具的互通项目收录，REA未确认。

补读作者11月19日22:50:11介绍帖与仓库11月19日UTC提交ac226de的README。文档描述匿名、未文档化网页API与JSON输出，查询无需账号或用户API key，内置约1400站，状态来自公开列车地图。它区分2027年1月25日前旧售票系统和之后新系统：旧系统失败会返回明确标注的部分列表，未知延误不是零，拦截和限流时停止。

项目报告11月17日旧系统Madrid–Barcelona有24车次、最低31.15欧元，以及新系统某次22车次与网页一致；这是文档中的项目检查，不是本合集实时票价或复现。购票支付有额外浏览器交互，不能把无账号查询写成无人确认付款。本合集未安装、调用Renfe、输入乘客资料或购票；MCP仍按候选标为进行中，补充回复“今晚可用”不是交付证明。补充介绍与文档早于严格窗口。

## 来源

- [Luis说明网页API研究与进行中MCP，2026-11-20](https://x.com/i/status/2123503882525454567)
- [补充：Renfe CLI作者介绍，2026-11-19](https://x.com/i/status/2123428629560320247)
- [补充：固定11月19日UTC提交的README](https://github.com/luisgonzaleznf/renfe-cli/blob/ac226dede6a5ad78543c8a7fd784e8f2b62fee00/README.md)

[English](en/renfe-cli-undocumented-web-api-agent-interoperability.md) | [返回目录](../README.zh-CN.md)
