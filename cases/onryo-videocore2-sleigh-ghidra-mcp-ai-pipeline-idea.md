# VideoCore II固件idea：先补SLEIGH解码，再让AI经MCP研究

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-05
阶段：待验证

2026年11月5日05:01:45（北京时间），Onryo（@3r1k4dl3r）提出：固件blob先经过定制VideoCore II SLEIGH解码器，进入Ghidra，再经MCP交给前沿AI自动逆向，最后独立验证并迭代。SLEIGH在这里是给Ghidra描述处理器指令的规格，MCP是Agent调用分析工具的连接层；连接模型不能自行补齐缺失的指令解码。

补查父串发现，11月3日23:14:11的根帖讨论树莓派签比特币交易是否安全，ynniv随后关注其中的二进制blob。11月5日04:44:15，ynniv说Ghidra甚至不支持VideoCore2，多数工具也不支持，Onryo才提出这条管线。05:14:43，ynniv回复已经在做，但不是REA。以上补充帖只用于背景与工具归属，不作为额外候选；没有据此声称ynniv执行了Onryo的完整方案。

没有固件版本、SLEIGH源码、指令覆盖表、反编译样例、模型名称或验证日志。独立验证只是方案中的要求，不能写成已验证的固件分析，更不能由讨论确认树莓派签名环境安全或发现后门。保留具体idea、unverified；未下载固件、执行目标或处理钱包与密钥。

候选封存0赞、21浏览、0转发；未用根帖传播量替代候选快照。

## 来源

- [候选：Onryo的VideoCore II／AI管线，2026-11-05 05:01:45](https://x.com/i/status/2118086322003030235)
- [补充根帖：树莓派交易签名背景，2026-11-03 23:14:11](https://x.com/i/status/2117636465811468353)
- [补充父帖：ynniv称缺少VideoCore2解码支持，2026-11-05 04:44:15](https://x.com/i/status/2118081917320872084)
- [补充回复：ynniv称正在做，但不是REA，2026-11-05 05:14:43](https://x.com/i/status/2118089581258064097)

[English](en/onryo-videocore2-sleigh-ghidra-mcp-ai-pipeline-idea.md) | [返回目录](../README.zh-CN.md)
