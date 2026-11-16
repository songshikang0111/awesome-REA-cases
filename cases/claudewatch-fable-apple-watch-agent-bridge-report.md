# ClaudeWatch腕上审批：darkzodchi报告Apple Watch与Mac Agent桥接

分类：硬件与设备互通 · 未确认使用 REA
记录日期：2026-11-16
阶段：待验证

2026年11月16日20:55:38（北京时间），darkzodchi（@zodchiii）称逆向自己的Apple Watch并装了Fable 5.2。帖文具体目标是手表上查看终端输出、接收文件修改／命令权限的震动提醒、点击批准或拒绝，以及发送语音指令；Claude Code继续在Mac上工作。

作者给的约10分钟设置流程涉及Bonjour发现Mac、skill/bridge中的Node中转、安装Claude Code hooks、六位配对码，以及ios/ClaudeWatch路径下用XcodeGen生成并签名iPhone／Watch目标。它支持把项目描述为手表与Mac Agent的控制桥，不能证明Fable模型在表上本地推理，也没有展示对watchOS二进制或私有协议的逆向过程。REA未提及，AI是否用于逆向本身也未明确。

补取原帖确认署名与步骤；仓库链接称在评论中，本合集未取得并审查源码、授权边界、配对安全或演示视频。约10分钟是作者估计，非实测。帖文建议关闭私有Wi-Fi地址，本文不据此建议读者降低隐私设置。未安装App或hooks、连接手表或执行命令，保留unverified的AI工具互通项目。

候选封存47赞、1403浏览、2转发、17回复；十分钟与功能为作者报告。

## 来源

- [darkzodchi的ClaudeWatch／Mac桥接介绍，2026-11-16 20:55:38北京时间](https://x.com/i/status/2122312640064352346)

[English](en/claudewatch-fable-apple-watch-agent-bridge-report.md) | [返回目录](../README.zh-CN.md)
