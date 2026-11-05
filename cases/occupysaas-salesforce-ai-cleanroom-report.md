# SalesCompel：OccupySaaS的Salesforce替代候选，文档明确未生产就绪

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-06
阶段：进行中

2026年11月3日09:14（北京时间），OccupySaaS转述同时点名Salesforce CRM替代，与Auth0身份目标分开记录。候选称AI、clean-room、Apache-2.0和drop-in兼容；这些不能据短帖升级为Salesforce完整替代或可直接迁移生产。

补查同组织salescompel固定提交2aa326536f38768c24744079398966d325bb6589的README，提交为10月22日01:10北京时间，早于本轮。项目称初步实现租户隔离的Go/PostgreSQL后端及Vue记录工作流，含Account/Contact CRUD、describe、有限查询、external-ID upsert与预配bearer认证。UI预览用合成数据，编辑仅在内存中、不调用后端，未实现入口禁用并标Planned。

截至文档10月20日进度，十一场景参考基线与局部walking slice获接受，Plan16记录两轮本地候选验收；但所有完整项目里程碑都没有exit-gate通过记录，且明确未做Salesforce兼容认证、未生产就绪。协议、安全、迁移、自动化与生产验证仍有大量工作。约185至350个额外plan equivalents只是项目范围估计，不是工时或交付日期。

2026年11月6日00:46:39的新候选再次把SalesCompel列为OccupySaaS的Salesforce替代项目，称目前只能建账号、读联系人，离可用仍有差距。此处建账号可能指CRM Account记录，不强解为已实现完整用户注册。新短帖没有固定提交、演示或测试，不能据概述否定旧README的有限API范围，也不把同帖ZeroAuthy的rc.1、提交数和代码量挪给SalesCompel。保留进行中且未生产就绪；未执行测试、连接CRM或读取客户数据。AI参与与被裁团队故事来自候选，项目文档不证明这些叙事。

11月3日共同候选快照0赞、20浏览、0转发；文档明确未作Salesforce兼容认证，参考基线不是候选全量验收。
11月6日共同候选封存2赞、141浏览、0转发；新摘要不是实测，不挪用ZeroAuthy版本或规模。

## 来源

- [OccupySaaS的AI重建Auth0／Salesforce转述，2026-11-03](https://x.com/i/status/2117425216573821238)
- [补充SalesCompel固定README，提交2026-10-21 UTC，早于窗口](https://github.com/occupysaas/salescompel/blob/2aa326536f38768c24744079398966d325bb6589/README.md)
- [新转述中的SalesCompel账号／联系人阶段，2026-11-06 00:46:39北京时间](https://x.com/i/status/2118384508743389461)

[English](en/occupysaas-salesforce-ai-cleanroom-report.md) | [返回目录](../README.zh-CN.md)
