# Stopwatch Micro：M5Stack StopWatch的非官方Codex Micro兼容固件与额度桥

分类：硬件与设备互通 · 未确认使用 REA
记录日期：2026-11-01
阶段：待验证

2026年11月1日09:56:53（北京时间），作者介绍Stopwatch Micro，把M5Stack StopWatch Dev Kit（ESP32-S3）刷成非官方Codex Micro兼容控制器，声称ChatGPT Desktop经蓝牙HID将其识别为Codex Micro。目标是离开键盘批准／拒绝、开新任务、切Agent对话与查看额度。帖子称C++加LVGL、MIT开源；六个按钮含Plan、Fast、Approve、Decline、New Task、Fork，弧形触控调推理强度，另有按住说话和发送按键。

作者明确额度不在Codex Micro协议中，因此另在Windows跑桥，从ChatGPT Desktop附带的Codex App Server取额度，再经蓝牙HID送到手表。其不需API Key、不复制登录token和可拔USB线均是项目自述，没有凭据或流量审计。额度两分钟未刷新标过期、十分钟不可用，而非继续显示新鲜数值，这是一项明确的数据新鲜度设计。

原帖称v0.4.0实机HAL自检17／17、控件13／13、50Hz传输151／151零丢包，提醒桌面更新可能使兼容层需要跟进。未取得可审代码、测试记录、固定版本或协议文档，不能把这些自测升级成独立复现或保证所有Desktop版本兼容。也未说明AI是否参与固件开发或具体逆向方法，作为面向AI工具的协议互通项目保留unknown，不推测REA。本合集未刷机、操作桌面客户端或访问任何登录材料。

候选快照2赞、86浏览、0转发；17／17、13／13、151／151均为作者自测，未审查日志。

## 来源

- [作者的Stopwatch Micro v0.4.0兼容固件报告，2026-11-01](https://x.com/i/status/2116711041413378459)

[English](en/stopwatch-micro-codex-hid-compatible-controller.md) | [返回目录](../README.zh-CN.md)
