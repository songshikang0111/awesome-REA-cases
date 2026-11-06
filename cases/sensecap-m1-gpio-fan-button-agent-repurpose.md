# SenseCAP M1继续服役：风扇与按钮GPIO研究交给Agent使用

分类：硬件与设备互通 · 未确认使用 REA
记录日期：2026-11-07
阶段：相关项目

2026年11月7日02:00:02（北京时间），brainstormity（@brainstormity）报告重新利用SenseCAP M1 LoRaWAN网关。作者称以62美元买到全新封装设备，内有四核Raspberry Pi4B、8GB内存、64GB高耐久SD卡、WM1302 LoRaWAN模块、金属壳、5V3A供电、风扇散热器、天线、安全元件与按钮，建议保留整机而非只拆树莓派。

改用Raspberry Pi OS后风扇与按钮默认不工作，作者称通过逆向定位风扇接GPIO13、按钮接GPIO27，可供开机／温控调速和自定义按钮行为，并给AI Agent准备Markdown协助文件。这建立研究结果交接给Agent的用途，未说明AI参与原始引脚定位，故不称REA或AI自动逆向。原帖补取确认作者，文件短链未读取。

每月0.90美元电费、压力测试不超过52°C及零件总值300美元以上均为作者说法，没有功率、环境温度、测试时长或市场估价核对。US915／EU868MHz传感器1–3英里安全系统是后续使用设想，不是已实现的LoRa部署。设备批次、电气安全、原系统恢复和全部硬件支持未验证；未刷卡、接设备、执行Agent文件或测试GPIO，按相关硬件互通项目收录。

封存7赞、498浏览、0转发；62美元、每月0.90美元、52°C与GPIO映射都是作者口径，非本合集实测。

## 来源

- [brainstormity的SenseCAP M1复用、GPIO与Agent文档自述，2026-11-07 02:00:02北京时间](https://x.com/i/status/2118765365123567760)

[English](en/sensecap-m1-gpio-fan-button-agent-repurpose.md) | [返回目录](../README.zh-CN.md)
