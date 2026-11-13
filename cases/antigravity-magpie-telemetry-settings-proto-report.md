# Antigravity遥测开关：用户称研究内部proto后由magpie代设，未核流量变化

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-13
阶段：待验证

2026年11月13日11:22:40（北京时间），@daoche_wuzui回复@magpie_router，称已实测magpie可使用已存OAuth token代设Antigravity的遥测开关，并说内部proto研究与实测在附图中。目标是AI开发工具的设置互通，帖子没有说明用AI辅助逆向，不能因目标是AI产品而假定REA或模型参与。

作者报告调用内部用户设置方法、将telemetryEnabled设为false，并说需要匹配客户端User-Agent以避免403，得到HTTP200及空userSettings对象。本合集不重复认证材料或实际执行请求；200只说明作者报告了一次接口响应，不证明读回值保持false、后续会话生效或所有遥测都停止。

补查确认作者、文字和图片附件，未审截图、完整proto、magpie代码、网络日志或持久化设置，亦未读取任何OAuth凭据、访问账户或发送写请求。作为具体AI工具互通研究报告收录，保留unknown／unverified，不将自述实测升级为独立验证。

候选快照0赞、11浏览、0转发、0回复；HTTP200和空设置对象为作者报告，未核遥测流量。

## 来源

- [daoche_wuzui的Antigravity内部proto与magpie遥测设置自测，2026-11-13 11:22:40北京时间](https://x.com/i/status/2121081282042139030)

[English](en/antigravity-magpie-telemetry-settings-proto-report.md) | [返回目录](../README.zh-CN.md)
