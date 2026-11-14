# GoGra Linux分析：Ghidra／OpenCode链路中四项反编译错误与两项AI错误

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-12
阶段：待验证

2026年11月12日10:22:02（北京时间），吉川孝志（@MalwareBibleJP）整理Fortinet研究者对GoGra Linux版的分析，称同题在Black Alps 2026报告。GoGra是通过Outlook邮件收发指令的后门；目标是伪装PDF的dropper中嵌入的剥符号Go载荷，不是重新实现邮件客户端。帖子把工具链描述为LLM经MCP操作Ghidra，配合OpenCode；未说明模型或REA。

据转述，LLM编写Ghidra脚本，从.gopclntab恢复函数名并定位OUTLOOKCLIENT包。研究者梳理六项错误，其中四项归于反编译器：漏显示getpid系统调用（AI评论反而正确）、漏掉SendingMessages调用、参数数量不对、Go字符串边界不对。后两项被归因于32位x86的Go栈传参约定与非NUL结尾字符串处理。两项AI错误是把返回用户名的GetClientName说成返回Linux，以及把dropper的Go build ID误认为Graph API bearer token。另有AES用途推断在研究者要求定位邮件处理代码前未给证据；这不是另算第七项已分类错误。

帖子还转述OAuth 2.0取Graph API令牌、读取删除Input主题邮件、Base64与AES-CBC处理后交Bash执行、加密结果由Output主题邮件发回的行为链。此处仅概述防御性分析结论，不提供载荷或可执行利用步骤。六项是该研究的观察，不是通用错误率。

本合集核对原帖正文与署名，未读到所链原文、会议材料、样本、脚本或完整分析输出；所有技术结论仍归因于这篇二手整理。AI与反编译器可能互相纠错不等于已自动验证结论。本合集未下载或执行恶意代码，也未连接邮件服务。

2026-11-12封存快照2赞、326浏览、0转发；四项反编译错误和两项AI错误是转述研究结果，不是独立复测。

## 来源

- [吉川孝志的GoGra Linux六项错误整理，2026-11-12 10:22:02北京时间](https://x.com/i/status/2120703635630051540)

[English](en/gogra-linux-ghidra-opencode-six-errors-report.md) | [返回目录](../README.zh-CN.md)
