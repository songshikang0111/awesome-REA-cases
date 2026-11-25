# gflow-cli接AI助手使用Flow积分：私有接口研究与真实浏览器限制

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-25
阶段：相关项目

2026年11月25日13:08:00（北京时间），Leonard.AI（@LeonardBuilds）因Ultra 5x每月1万Flow积分，比较让Antigravity点击网页与ffroliva/gflow-cli的CLI／MCP路线。他称后者通过本地Playwright保存登录状态、调用Google内部接口，支持并发、批量、串镜头和角色复用，跑起来比点网页快；同时提醒私有接口易变化、并发可能触发账号风控。速度与套餐数字是作者自述，无计时或账户核验。

补读公开项目README，核对到它是独立于Google的Python CLI和MCP服务，面向Claude Code／Desktop、Cursor、Codex等客户端，使用用户自己的Flow会话与积分。重要更正：所读文档将当前生产传输明确写为ui_automation，即持久Playwright配置里的真实有头Chrome；纯HTTP视频受401与reCAPTCHA阻碍，旧HTTP策略留在experimental，不在生产路径。因此不能把候选的接口描述写成已摆脱浏览器、无头可用或可无限水平并发。读取的是补充时main文档，未固定提交或核对文档原始日期，不冒充候选发布时的版本。

文档称项目beta、默认Claude插件禁用，MCP的no-spend模式不注册消耗积分的工具；这些是项目声明，未读源码或消费审计、未复跑其逐版真实Flow验证。作者另提官方Gemini API每月40美元赠金用API额度而非Flow积分，仅作为其选择背景，不认证订阅权益。该工具把非官方接口／浏览器自动化接给AI，是相关项目，不证明AI编写了逆向实现或使用REA。未安装、登录、读取Cookie、生成媒体或触碰账户。

候选封存0赞、112浏览、0转发、1回复；未计时，不将作者的更快描述量化。

## 来源

- [Leonard.AI比较Antigravity与gflow-cli的Flow自动化及风险，2026-11-25 13:08:00北京时间](https://x.com/i/status/2125456445231538475)
- [补充公开README：真实Chrome生产传输、HTTP限制与积分护栏；本次读取main，文档原日期未核](https://github.com/ffroliva/gflow-cli/blob/main/README.md)

[English](en/gflow-cli-flow-private-api-agent-integration.md) | [返回目录](../README.zh-CN.md)
