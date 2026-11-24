# 1998年的LightLink重新亮起：Claude读旧固件与电路图，人类换控制器并纠线

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-24
阶段：待验证

2026年11月24日02:47:43（北京时间），媒体作者转介Larry Pesce的1998年LED招牌复活项目。补读Bill Brenner的CYBR.SEC.Media报道与Pesce本人11月23日Secure Ideas原文，二者早于本轮窗口，只作追溯。目标为Inova LightLink CFM16.200S-IP，200×16红绿双色显示屏；Pesce在DEF CON购入后因专有软件与未文档化以太网协议而闲置至少十年。这里不是破解原网络协议：他绕开原控制器，直接驱动显示面板。

Pesce称Claude根据设备照片找到Yadid Ramot的2015年项目，读取其PIC固件和Eagle原理图，重建扫描、时钟与排线引脚，辨认5V的74HC244与ESP8266的3.3V电平不匹配，提出电平转换。Claude再编写定时显示驱动、Wi-Fi配置、网页预览、文本播放列表、REST API、FSEQ灯光序列播放和OTA固件。作者称助手遇PlatformIO网络障碍后另取工具链完成编译、对照FSEQ规范；这些是项目报告，本合集未执行构建。

首次实机出现上半屏缺绿色等现象，Pesce给照片，Claude建议检查绿色数据线；作者发现误接地，移动一根跳线后报告正常。人类负责器件、接线、测量、通电和判断，也曾发现模型漏项，不能称AI独立修好。后续Claude以KiCad API生成通孔PCB，第三方自动布线程序受限后自写两层迷宫路由，并报告DRC通过；原文明确板子尚未制造或实测。一个下午只指PCB设计阶段，不是全部复活工时。公开仓库链接见原文，未审代码、二进制或完整检查记录，未下载执行或连接硬件。拟用于显示自动化IoT测试任务状态，REA使用未明；保留未独立核验状态。

候选封存1赞、57浏览、0转发、0回复；至少十年为闲置时间，一个下午为PCB设计自述，不是完整项目计时。

## 来源

- [候选：媒体作者介绍Larry Pesce项目，2026-11-24 02:47北京时间](https://x.com/i/status/2124937961007706132)
- [补充第一方：Pesce的研究、实机纠线与未制造PCB，2026-11-23，窗口前](https://www.secureideas.com/teaching-a-1998-led-sign-new-tricks-with-an-ai-riding-shotgun/)
- [补充媒体报道：Bill Brenner，2026-11-23，窗口前](https://www.cybrsecmedia.com/ai-helps-security-researcher-bring-1998-led-sign-back-to-life/)
- [第一方原文链接的公开固件与PCB仓库；未执行或逐项审计](https://github.com/AppliedMalice/lightlink-esp8266)

[English](en/larry-pesce-lightlink-1998-claude-controller-revival.md) | [返回目录](../README.zh-CN.md)
