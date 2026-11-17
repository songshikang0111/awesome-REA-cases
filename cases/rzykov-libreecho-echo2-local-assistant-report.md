# 二手Echo 2刷LibreEcho：Roman报告本地模型选择与SSH，Codex连接仍失败

分类：硬件与设备互通 · 未确认使用 REA
记录日期：2026-11-18
阶段：相关项目

2026年11月18日00:14:34（北京时间），Roman Zykov（@rzykov）因不满Alexa体验，买二手Amazon Echo第二代，拆机焊USB并利用已有漏洞刷LibreEcho。他说除ChatGPT Codex订阅连接外其余能用，SSH也可用，看重可完全使用本地模型的选择。保留为设备再利用与AI互通的相关项目，不把笼统其余能用写成所有功能通过测试，也不声称本地LLM在Echo本机完成推理。

补充读取aslater3/LibreEcho固定9e5b716 README，提交2026-11-17 13:51:23 UTC，早于候选。文档列Echo 2与Echo Dot 2、MT8163上的Linux 6.1、本地唤醒／语音识别／合成及可选本地LLM端点、Home Assistant与可选SSH；明确Dot较少实机测试，新机型只是研究路线。它将安装依赖的Amonet／Kaeru解锁归功于Roger Ortiz、k4y0z等既有研究，不能把Roman刷机当其原创漏洞或AI自主破解。

README还披露每周匿名设备统计ping，0.14.5起可关；健康等选项默认勾选但文档称该版本只记选择不发送对应数据。因此本地优先不等于已验证零外连或隐私保证。旧启动链迁移完整写入未端到端实测；本合集不复述刷写步骤，也未执行脚本、接设备或检查网络。未审演示、完整代码与会话；没有证据表明AI参与逆向过程，REA和工程模型均未知，Codex故障仍按作者报告保留。

2026-11-18封存3赞、79浏览、0转发、1回复；没有工时、全面兼容或独立隐私测试。

## 来源

- [Roman的二手Echo 2／LibreEcho报告，2026-11-18 00:14:34北京时间](https://x.com/i/status/2122725090349502912)
- [候选前固定LibreEcho README，提交2026-11-17 13:51:23 UTC](https://github.com/aslater3/LibreEcho/blob/9e5b7165a5f137a91d353abdec8af4eaac0dc5f2/README.md)

[English](en/rzykov-libreecho-echo2-local-assistant-report.md) | [返回目录](../README.zh-CN.md)
