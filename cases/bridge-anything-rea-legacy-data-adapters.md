# Bridge Anything：用REA映射无API旧软件的数据，再做REST／MCP／CLI桥接

分类：应用与客户端 · REA
记录日期：2026-11-21
阶段：相关项目

2026年11月21日22:27:35（北京时间），Viho.AI（@Viho_Huangg）介绍Artesiana的bridge-anything。它面向诊所、经销商和旧ERP这类没有开放API、数据留在后台服务器的软件，提出让REA研究安装目录及读写方式，在旁边建桥，以REST、MCP与CLI供自己的应用访问，而不是让业务应用直接依赖旧数据库。

帖子给出七步：核实授权，找数据位置，对每块数据做一次操作一次数据库差分并与界面对照，选择访问路径，建立并测试桥接，接入应用，最后可选分享至OpenCoupler。拟保留BRIDGE.md、UNKNOWNS.md、DATA-PROTECTION.md以记录映射、疑点和个人数据。它特别反对猜表名后直接生产写入。

11月22日补读公开README，确认项目宣称支持Claude Code、Codex、Cursor等Agent，以REA分析数据访问代码；列举SQL Server、Firebird、SQL Anywhere、Btrieve、Access、dBase、SQLite等识别对象，路径优先厂商API、接口文件、只读数据库、UI自动化，写入仅走原软件使用的路径，测试使用匿名快照。诊所预约示例只是提示词，不是已交付的客户实现。文档要求有许可或书面同意、只分析副本，不绕过许可检查、DRM、加密凭据或访问控制；这些是规定，不证明每次运行都遵守或所有映射都被验证。

所读README没有固定提交或原始发布日期，只作为窗口候选的补充项目资料；未读完整技能、源码或测试，没有运行Agent、连接数据库或接触个人数据。保留为具体互通方法与相关项目，不称已有经核验桥接产品；功能与安全边界仍待实际验证。

11月21日候选快照：0赞、39浏览、0转发、0回复；README为后续阅读的可变文档，未运行技能或复测桥接。

## 来源

- [Viho.AI的Bridge Anything流程介绍，2026-11-21 22:27北京时间](https://x.com/i/status/2124147716725096742)
- [Artesiana公开README，11月22日补读，原始更新日未核](https://github.com/Artesiana/bridge-anything/blob/main/README.md)

[English](en/bridge-anything-rea-legacy-data-adapters.md) | [返回目录](../README.zh-CN.md)
