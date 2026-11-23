# 16英寸M5 Pro跑Omarchy：Julian Arango称Claude辅助修安装器与Wi-Fi

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-23
阶段：进行中

2026年11月23日07:20:59（北京时间），Julian Arango（@ja818_）称用一个周末与Claude Code让Omarchy原生运行在16英寸MacBook Pro M5 Pro。他说omarchy-m5文档尚称不支持16英寸，自己修改安装器允许该型号，14英寸镜像无需改动即可启动，使用Apple普通27.2固件、无macOS beta，并能用全部18个CPU核心。这是作者的设备适配报告，不是本合集核实的Apple规格或完整驱动实现。

作者称Wi-Fi初始不出现，原因是16英寸设备树一行无限等待Linux尚未设置的电源引脚，删除该行后Wi-Fi出现；连接家用路由器仍报错误密码，随后修复驱动拒绝WPA／WPA2混合模式的问题并送上游。自报键盘、触控板、Wi-Fi、蓝牙、USB、合盖睡眠与电池可用，声音、GPU与相机是下一步目标。该具体兼容性调试归广义AI辅助硬件研究，不声称从闭源固件还原驱动，也不与其他人的Mac或Shield移植混为同一项目。

补取原帖确认署名与两张图片附件，未查看图片、仓库、差异补丁、上游接收记录、启动日志或稳定性测试。一个周末为回顾工时，送上游不代表已合并，能启动也不等于所有硬件可用。保持in-progress；未安装系统或执行项目，REA未提。

封存快照1赞、23浏览、0转发、1回复；一个周末、18核心及27.2固件均为作者所述，未核补丁或实机。

## 来源

- [Julian Arango的16英寸M5 Pro／Omarchy与Claude Code适配报告，2026-11-23 07:20:59北京时间](https://x.com/i/status/2124644341129888078)

[English](en/julian-arango-16inch-m5-pro-omarchy-claude-report.md) | [返回目录](../README.zh-CN.md)
