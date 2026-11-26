# ReliableSite的BMC原生AI接口：Radic Davydov报告硬件级computer use

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-26
阶段：待验证

2026年11月26日05:49:28（北京时间），Radic Davydov（@RadicDavydov）称ReliableSite已逆向他们所用全部硬件厂商的BMC，并通过自建AI harness提供原生访问，使computer-use功能直接作用在硬件层。BMC即服务器基板管理控制器，负责带外管理；其目标是把硬件管理能力变成Agent可直接调用的接口，而非靠屏幕点击。

全文没有厂商清单、控制器版本、协议映射、工具定义、权限隔离、审计日志或操作演示。全部只指作者所说的自有部署范围，不是市售所有BMC；AI明确用于最终harness，是否也参与此前逆向没有说明。补取确认署名与文字，未审源码或接服务器，不据此确认越权访问、通用兼容或生产安全。REA未提。

封存2赞、137浏览、0转发、1回复；覆盖范围为作者声称的所用硬件。

## 来源

- [Radic Davydov的ReliableSite BMC与AI harness自述，2026-11-26 05:49:28北京时间](https://x.com/i/status/2125708473669206267)

[English](en/reliablesite-bmc-native-ai-harness-report.md) | [返回目录](../README.zh-CN.md)
