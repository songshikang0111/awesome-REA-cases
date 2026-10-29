# 自购5G Wi-Fi路由器：Onur Solmaz报告DeepSeek发现空密码与API注入

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-10-30
阶段：待验证

2026年10月30日00:00:06（北京时间），Onur Solmaz（@onusoz）报告让opencode go订阅中的普通DeepSeek检查新买的5G Wi-Fi路由器，称SSH接受空密码，管理面板HTTP API的测试页面可造成shell注入。他把问题称为零日，目标是发现并加固自己设备上的漏洞；未明确说使用REA，帖子中的Reverse Engineer Anything表述不能替代工具调用证据。

作者明确说攻击者需要先连接他的Wi-Fi，并担心之后安装间谍软件；这不是已观察到入侵或流量窃取的记录。帖子未公开厂商、型号、固件版本、漏洞编号、厂商确认或修复测试，空密码是否为默认配置及零日属性均未独立核实。他关于旧设备普遍不安全的推论不是本案例测量结果。本合集仅核对原帖署名和正文，未连接路由器、执行注入或验证漏洞，保留unverified。

候选快照109赞、4562浏览、4转发；补查时浏览量变化，不覆盖候选快照。

## 来源

- [Onur Solmaz报告DeepSeek检查自购路由器，2026-10-30](https://x.com/i/status/2115836080960508083)

[English](en/deepseek-opencode-5g-router-security-report.md) | [返回目录](../README.zh-CN.md)
