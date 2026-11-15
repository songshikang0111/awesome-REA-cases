# Litra Glow灯不装G HUB：Manuel Bieh称Claude做出约2MB菜单栏控制器

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-15
阶段：待验证

2026年11月15日19:30:01（北京时间），Manuel Bieh（@ManuelBieh）介绍自己的Logitech Litra Glow摄像补光灯。他只想开关灯和调光，不想安装约1GB的G HUB，称让Claude研究USB协议，写成约2MB的macOS菜单栏应用。作者回忆开发中灯突然亮起并变化，报告可调亮度、色温和开关，右键图标快速切换；这是作者实机经历，不是本合集复现。

原帖短链确认指向manuelbieh/litra-glow-controller。补读固定641005a63a97daeeea8637922672b75ca3f9af97 README，提交为2026年10月25日03:58:54 UTC，早于窗口，只作项目背景。文档确认USB HID、20—250 cd/m²亮度、2700—6500K色温、可选登录启动与附带litra.py脚本；要求macOS13及以上，分发为ad-hoc签名。数值是软件文档的控制范围，不是本合集光学测量。

重要归属差异：README明确使用开源社区已逆向的协议，因此不将Claude写成从零独立发现全部USB指令。README把G HUB说成500多MB，帖子说约1GB，两者是不同来源的近似口径，未测安装或运行占用；约2MB也仅为作者说法。固定提交有Claude Opus5.5协作署名，只支持该补丁归属，不证明整个协议研究的完整模型轨迹。项目称MIT、非Logitech官方。本合集未下载二进制、运行脚本、安装应用或连接灯，REA未提及，保持unverified。

封存候选1赞、15浏览、0转发、2回复；没有开发工时。
约1GB与约2MB为作者近似数值，README另称G HUB500多MB；未做同条件大小或内存比较。

## 来源

- [Manuel Bieh的Claude／USB与约2MB控制器报告，2026-11-15 19:30:01北京时间](https://x.com/i/status/2121928704376885636)
- [窗口前固定README：功能范围、USB HID与社区协议归属，提交2026-10-25 03:58:54 UTC](https://github.com/manuelbieh/litra-glow-controller/blob/641005a63a97daeeea8637922672b75ca3f9af97/README.md)
- [同一固定提交的Claude协作署名与安装路径补丁](https://github.com/manuelbieh/litra-glow-controller/commit/641005a63a97daeeea8637922672b75ca3f9af97)

[English](en/manuelbieh-litra-glow-claude-usb-menubar-controller.md) | [返回目录](../README.zh-CN.md)
