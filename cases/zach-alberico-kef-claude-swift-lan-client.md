# KEF LSX II菜单栏客户端：Zach让Claude参考Python协议并查实机差异

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-25
阶段：待验证

2026年11月25日00:29:47（北京时间），Zach Alberico（@zalberico）解释自己的KEF音箱客户端：Claude并非抓包KEF Connect，而是参考开源Python库pykefcontrol，按局域网HTTPS JSON API写原生Swift实现，涉及getData／setData、实时事件队列与HMAC签名写入。补读同日00:18:20的父帖只作背景：目标是KEF LSX II，作者不喜欢iOS官方App，称让Claude一夜写出macOS菜单栏替代端。这不是本轮另一个候选，也不是完整逆向官方App的证据。

作者报告先读后写测试自己的音箱，在固件3.1.141上只有HTTPS 4430服务、80端口关闭；频繁新建连接会出问题，所以客户端复用一条连接，开关状态要看当前输入而不是可能过时的status字段。这些是作者报告的设备观察，未给请求记录、源码或其他型号测试；分享代码只是意愿。本合集未连接设备、验证HMAC或运行客户端；一夜是父帖自述，不是独立计时。与roberdorfer的USB音频透传／细音量桥为不同实现，不能借用其延迟和采样率指标；未提REA。

候选封存1赞、14浏览、0转发、0回复；仅作者自有设备观察，非独立复现。

## 来源

- [候选：Zach说明Claude参考pykefcontrol与固件差异，2026-11-25 00:29:47北京时间](https://x.com/i/status/2125265634783281444)
- [补充父帖：LSX II与macOS菜单栏替代端，2026-11-25 00:18:20北京时间，非另一个候选](https://x.com/i/status/2125262753078383040)

[English](en/zach-alberico-kef-claude-swift-lan-client.md) | [返回目录](../README.zh-CN.md)
