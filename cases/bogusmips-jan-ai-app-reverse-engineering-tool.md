# BogusMips：Jan把Android包、smali与网络流量交给内置AI分析

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-01
阶段：相关项目

2026年11月1日03:57:04（北京时间），Jan（@derjanni）以作者身份介绍App逆向多工具BogusMips。补读jankammerath/BogusMips固定提交dba5f409f2594437d9f113281b42f7c768fd918b的README；提交时间为2026-10-31 19:43:55 UTC，早于候选。工具以Rust写成，打开APK／XAPK，展示DEX的smali、解码Manifest与资源、搜索并导出内容；不应误写成已恢复原始Java源码。

文档中的AI面板支持Grok、Gemini、Claude、OpenAI和自定义兼容端点，能通过包搜索／节点读取／网络流量工具结合静态内容作分析。Network视图用Android模拟器与内置代理采集HTTP／HTTPS，HTTPS要求可root映像与信任证书；Chrome Root Store、证书固定和Google服务仍有限制。可配置Frida脚本，但文档说明早期启动检查、原生检测、服务端完整性认证不能保证绕过，预览Android版本可能不支持。

这是公开文档可辨的集成工具，不是已破解某个商业App的案例。这里未安装、运行模拟器、改证书、调用模型或采集流量，也未验证解析器兼容率、解密覆盖或平台支持。

候选快照0赞、2浏览；文档核读，未运行工具。

## 来源

- [Jan介绍BogusMips的原帖，2026-11-01](https://x.com/i/status/2116620489061707869)
- [补充项目README：固定提交的解析、AI与网络边界](https://github.com/jankammerath/BogusMips/blob/dba5f409f2594437d9f113281b42f7c768fd918b/README.md)

[English](en/bogusmips-jan-ai-app-reverse-engineering-tool.md) | [返回目录](../README.zh-CN.md)
