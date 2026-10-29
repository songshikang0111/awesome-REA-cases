# scapectl：Claude Code辅助恢复Fractal Scape耳机USB协议与跨平台控制器

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-10-29
阶段：进行中

2026年10月29日22:14:21（北京时间），Jamie Dubs（@jamiew）介绍Fractal Design Scape无线游戏耳机的非官方配置器scapectl，称来自AI逆向及反复测试。同作者父帖称v0.0.17新增菜单栏状态、吊杆麦克风事件、接收器插拔处理和单次低电提醒。补读charlietran/scapectl固定提交945ee25cda7487516a1ee0d02b436bff1923e457的README；提交时间同日14:06:03Z，早于发帖。文档明确致谢Claude Code帮助理解USB协议和实现跨平台Go应用，REA未提及。

协议研究来自Adjust Pro网页的WebHID流量及Electron应用源码，不是AI从零猜协议。公开文档记录USB接收器与耳机中继区别、状态轮询、EQ和麦克风控制；还指出某接收器存在字段不可靠，以及源码中麦克风布尔含义与实机相反，需要以设备行为修正。应用提供电量/麦克风等状态、EQ预设切换、RGB与降噪开关及事件触发外部脚本；音频输出切换仍依赖另外的工具。

README只称macOS和Windows已测试；Linux是构建目标，不是已完成实机验证。蓝牙连接检测、完整灯效、按钮自定义和EQ导入导出仍列计划。不能与Adjust Pro同时占用同一HID流；macOS未经公证、Windows未签名，项目GPLv3并注明上游依赖。本合集只读文档，未安装、取消系统保护、连接耳机或复测协议，保留进行中状态。

候选快照0赞、30浏览、0转发；父帖与仓库为同日补证。
公开协议与实现不等于独立设备复测；Linux未实测，macOS未经公证、Windows未签名。

## 来源

- [Jamie Dubs称scapectl来自AI逆向与测试，2026-10-29](https://x.com/i/status/2115809467967180976)
- [补充：同作者v0.0.17更新父帖，2026-10-29](https://x.com/i/status/2115809465224294886)
- [补充：scapectl固定README、协议参考与平台限制，2026-10-29提交](https://github.com/charlietran/scapectl/blob/945ee25cda7487516a1ee0d02b436bff1923e457/README.md)

[English](en/scapectl-fractal-scape-claude-usb-hid.md) | [返回目录](../README.zh-CN.md)
