# Privy CLI：从控制台请求恢复接口，供Agent管理开发账号

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-10-30
阶段：相关项目

2026年10月30日22:59:42（北京时间），Samarth（@awesamarth_）发布@awesamarth/privy-cli，称把Privy开发者控制台的API提供给Agent，可创建应用、配置登录方式、取分析数据与管理用户。22:59:43后续候选解释逆向实际是分析控制台到后端的网络请求并纳入CLI，灵感来自Cloudflare cf与Stripe CLI；没有说AI执行了协议研究，rea记unknown，按服务Agent的逆向接口相关项目收录。

同串补充明确它不是Privy的Agent钱包CLI，而是管理Privy账号；声称因缺少设备码式CLI授权路径做了workaround，但候选未解释细节。公开npm元数据确认0.1.0发布于2026-10-30T13:48:46.526Z并指向awesamarth/privy-cli。补读固定提交7662742e327cf1b39b270845113d487b8c67b277的README，提交14:04:09Z，均在本窗口内但仅为补充证据，不另算候选。

README要求Node.js22.18+和已解锁OS凭据库，说明直连HTTPS、多数管理接口未文档化且可能变化。新登录要浏览器CAPTCHA与隐藏终端邮箱码，已存会话可尝试续期；文档另有可选共享会话导入，不把这些机制称为破解认证。默认JSON输出，提供发现、schema、预览/差异、显式执行和回读验证；dry-run是离线校验，不等于远端成功。写操作不自动重试或回滚，超时后需先读状态。

管理范围涵盖用户、钱包、策略、webhook、客户端、配置与分析，不支持钱包签名/交易、私钥导出、所有者批准执行等。配置回读也不能证明真实第三方登录、DNS、webhook或钱包部署成功。项目称非官方、无Privy背书；npm存在和文档不能证明全部端点可用或账号安全。本合集未安装依赖、登录、访问凭据、调用管理API或执行任何变更，只静态检查公开材料。

主候选快照8赞、145浏览、0转发；后续1赞、17浏览、0转发。
0.1.0发布与固定提交均早于候选但在本窗口；未运行CLI或验证远端端点。

## 来源

- [候选：Samarth发布Agent友好Privy管理CLI，2026-10-30 22:59:42](https://x.com/i/status/2116183267275911517)
- [候选后续：控制台网络请求研究及授权限制，22:59:43](https://x.com/i/status/2116183270605873329)
- [补充：同作者区分管理账号与Agent钱包CLI，22:59:43](https://x.com/i/status/2116183273793790210)
- [补充：固定README，登录、确认与验证边界，10月30日提交](https://github.com/awesamarth/privy-cli/blob/7662742e327cf1b39b270845113d487b8c67b277/README.md)
- [补充：npm发布元数据](https://registry.npmjs.org/@awesamarth/privy-cli)

[English](en/privy-cli-dashboard-api-agent-management.md) | [返回目录](../README.zh-CN.md)
