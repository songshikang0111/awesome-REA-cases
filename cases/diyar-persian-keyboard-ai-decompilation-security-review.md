# Diyar波斯语键盘：M.A.H称反编译后用AI审视输入服务风险

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-04
阶段：待验证

2026年11月4日20:40:31（北京时间），M.A.H（@DevUranium）在围绕Diyar的争议中报告反编译该波斯语键盘助手，并用AI解释架构。作者说拆开WiX Burn安装包、查看MSI数据库、解开cab1／cab2／cab3，把.NET9二进制恢复为C#，并计划在GitHub发布供别人检查。补取仅确认署名和全文，没有取得可确认仓库或分析产物，不把发布计划写成已公开源码。

作者称看到SetWindowsHookEx／WH_KEYBOARD_LL、Named Pipe及TSF事件，认为CoCoTextService.dll作为文本服务会进入其他进程；又称密码字段过滤是脆弱启发式、文件无Authenticode签名。他把这些归为高风险双用途架构，担心密码进入内存缓冲。与此同时，帖子明确说AI并未将其判为木马、勒索或窃密软件，作者没有发现秘密服务器、外传口令或隐藏webhook，只报告更新检查和用户配置密钥后的Azure翻译连接。

这些均为作者及其AI的静态解读，不是本合集认证安全或恶意。TSF和键盘hook存在不能单独证明窃听、密码泄漏或感染所有进程；未给版本、哈希、权限路径、运行抓包、签名检查结果或独立审计。所列源码行号只是作者定位，不在此验证。AI型号和REA未说明，附件图未检查，未下载反编译代码或运行程序。

封存快照0赞、11浏览、0转发；Riskware及无外传判断都是作者观点，不是独立鉴定。

## 来源

- [M.A.H的Diyar反编译与AI架构分析，2026-11-04](https://x.com/i/status/2117960180906275128)

[English](en/diyar-persian-keyboard-ai-decompilation-security-review.md) | [返回目录](../README.zh-CN.md)
