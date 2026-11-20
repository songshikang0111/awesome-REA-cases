# PicPak电子墨水相框：Claude辅助固件与自托管替代，项目仍进行中

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-20
阶段：进行中

2026年11月20日22:00:10（北京时间），whyamas（@whyamas）转述@iGottZ研究云绑定电子墨水相框，并用Claude写替代ESP-IDF固件与自托管后端，明确只部分完成。补查找到Jan-Stefan Janetzky（GottZ）的open-PicPak公开仓库，固定提交7b76daab2219b0a1c061fbe9fbf91747a8961954为7月14日17:37:28北京时间；旧项目文档作为目标背景补证，不是本窗口新发布成果。

README把设备定义为ESP32-C3、4.2英寸400×300黑白红黄屏，原厂仅BLE，手机App需从云取图再推送。项目报告研究硬件、GATT／OTA与RGB到面板管线，自报一天做出Home Assistant WiFi拉图相框，之后加入按图变化刷新、低电量门控、恢复保护与Berry渲染配置。一天属于项目说法，不是完整平台开发工时。

文档将固件、后端与工具标为进行中，Web-USB未公开；原App兼容BLE重实现与播放列表仍计划中，operator TUI机上验证待做。部分恢复保护写有机上验证，也不能覆盖全部功能。候选提供Claude归因，README本身不证明每项AI参与。只读README，未审协议全文、运行代码、连接相框或验证安全、续航、OTA与账号；不把clean-room自述当法律结论，REA未提及。

候选封存0赞、6浏览、0转发、0回复；一天、恢复验证与功能均为项目报告，未实机检查。

## 来源

- [whyamas转述iGottZ的Claude相框项目，2026-11-20 22:00:10北京时间](https://x.com/i/status/2123778432186429613)
- [补充旧项目README：2026-07-14 17:37:28北京时间固定版本](https://github.com/GottZ/open-PicPak/blob/7b76daab2219b0a1c061fbe9fbf91747a8961954/README.md)

[English](en/igottz-eink-frame-claude-selfhosted-firmware.md) | [返回目录](../README.zh-CN.md)
