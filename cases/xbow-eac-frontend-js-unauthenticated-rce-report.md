# EAC公开应用：Jhaddix转述XBOW Agent研究前端JS并报告未认证容器RCE

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-12
阶段：待验证

2026年11月12日23:41:29（北京时间），JS0N Haddix（@Jhaddix）明确感谢当周赞助商XBOW，转述其自主AI Agent在美国Election Assistance Commission（EAC，选举援助委员会）所属公开应用发现Critical级未认证远程代码执行。帖子称Agent逆向前端JavaScript、沿攻击路径验证后端容器中的root代码执行，并称已负责任披露、在11月3日选举前修补。

具体研究对象是一个公开应用，不等于选举计票、投票机或全机构网络；容器root也不自动等于宿主机权限。Critical等级、可利用性、修补与披露时间都是赞助转述，没有应用URL、漏洞编号、补丁或复测材料供本合集确认。帖子有详细报告链接，但本合集未取得该报告，不补造攻击链或确认受影响范围。

补取只核对署名、正文与赞助关系，没有访问目标、运行利用、查看凭据或取得任何数据。REA未提及，归other-ai；保留unverified，不把厂商报告或推广背书升级为独立复现，也不将来源发布日期当作漏洞发现日。

封存13赞、1556浏览、3转发、1回复；修补早于11月3日是原帖主张，非本合集核验。

## 来源

- [Jhaddix披露XBOW赞助关系的EAC应用漏洞转述，2026-11-12 23:41:29北京时间](https://x.com/i/status/2120904824757850134)

[English](en/xbow-eac-frontend-js-unauthenticated-rce-report.md) | [返回目录](../README.zh-CN.md)
