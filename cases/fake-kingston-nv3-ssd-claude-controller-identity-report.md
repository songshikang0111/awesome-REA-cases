# 假Kingston NV3的身份检查：Claude先误判，再查控制器与固件的转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-17
阶段：待验证

2026年11月17日01:45:01（北京时间），Vaibhav Sisinty（@VaibhavSisinty）转述一位Reddit用户购买SSD的经历：本来订2TB，收到显示4TB的盘以为赚到；Windows和SMART报健康，但Claude Code花数小时扫描、格式化和缩小批次重试，仍说硬件坏。用户追问是否真是D盘并要求研究问题后，Claude改查设备自报身份。

帖文称控制器为Realtek而不是其认为真Kingston NV3应有的Silicon Motion，序列号带Realtek标识，固件也对不上真NV3；标4TB的盘实际据称约256GB。这里是AI辅助检查设备身份与故障解释的相关硬件分析，不是反编译SSD固件，也没有公开验证某批次真盘控制器配置。型号与假盘结论归于二手来源，不据此提供单一控制器品牌的通用真伪规则。

补取确认发帖者及正文和图片附件；未读原Reddit帖、SMART输出、控制器ID、固件、序列或容量测试，亦未审图片。数小时不是工时日志，约256GB未独立测量；尤其保留Claude前期误判和人的质疑，不写成Agent自行一遍识破假盘。未连接磁盘或执行格式化，保持unverified。

候选封存8赞、1977浏览、0转发、5回复；4TB、订购2TB及约256GB均为转述。

## 来源

- [Vaibhav Sisinty转述Claude检查假NV3身份，2026-11-17 01:45:01北京时间](https://x.com/i/status/2122385465664037284)

[English](en/fake-kingston-nv3-ssd-claude-controller-identity-report.md) | [返回目录](../README.zh-CN.md)
