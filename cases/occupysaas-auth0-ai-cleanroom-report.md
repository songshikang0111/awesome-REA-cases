# zeroauthy：OccupySaaS的Auth0兼容身份服务，完整替代仍是目标

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-03
阶段：进行中

2026年11月3日09:14（北京时间），一篇英文帖称被裁工程师组成OccupySaaS，用AI clean-room重建Auth0与Salesforce，Apache-2.0且drop-in兼容。本条只记录Auth0身份认证目标；失业经历、AI参与程度与替代雇主的动机来自帖文，未取得团队独立证明。

补查occupysaas组织确认zeroauthy仓库，阅读提交5d1c30c1ac7c90d88307c1958af7d7fd20ef0d54的README，提交为11月2日14:56北京时间，早于窗口。项目称从公开文档与开放标准独立实现Auth0 Authentication/Management API，可自托管，列出发现/JWKS、授权码加PKCE、刷新令牌、管理台、组织与事件流等能力，并报告用auth0-spa-js、auth0-react、nextjs-auth0及auth0-cli验证部分路径。

README声明OpenID Foundation的Basic、Config、Form Post OP三种profile已认证，批准日期10月30日，但本合集未另查认证名录；即便认证属实，也不代表Auth0全功能兼容。文档仍标early，MFA、无密码与电话、更多企业协议、生产加固等列为后续，迁移也有排除项。AI归因来自候选，功能与测试来自项目，不能互相升级为独立复现。未构建、登录或接触任何真实身份凭据；Apache-2.0是项目声明，不作clean-room法律合规鉴定。

共同候选快照0赞、20浏览、0转发；OpenID认证为项目声明，未另行核对。

## 来源

- [OccupySaaS的AI重建Auth0／Salesforce转述，2026-11-03](https://x.com/i/status/2117425216573821238)
- [补充zeroauthy固定README，提交2026-11-02，早于窗口](https://github.com/occupysaas/zeroauthy/blob/5d1c30c1ac7c90d88307c1958af7d7fd20ef0d54/README.md)

[English](en/occupysaas-auth0-ai-cleanroom-report.md) | [返回目录](../README.zh-CN.md)
