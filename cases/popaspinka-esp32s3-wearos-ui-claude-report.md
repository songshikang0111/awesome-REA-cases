# ESP32-S3圆屏重建Wear OS界面：PopaSpinka的Claude驱动与样例移植转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-25
阶段：待验证

2026年11月22日02:16:34（北京时间），RetroChainer转述YouTube作者PopaSpinka的项目：40美元Waveshare ESP32-S3、466×466圆形AMOLED且无GPU，原厂滚动图标撕裂，不能手指拖动。帖子称开发者不用LVGL或Arduino_GFX，借Claude Code从头写显示、触摸驱动和绘图库，再由Opus5.5移植Google开放Wear OS样例，含滚动数字、Pixel Watch式卡片、天气和音乐界面。

两天两个晚上、60fps、零丢帧、零撕裂、静止时零绘制均为该帖转述；3:22原厂撕裂与4:16标准驱动闪烁是作者给的影片位置，未观看或测量。本项目是已有开放样例及设备行为的改造，不是破解Pixel Watch或以40美元复刻Google收购的全部技术。

补读回复，有人询问电池唤醒首帧，未见测试答复；不把少绘制自动升级为已测续航。未取得仓库、代码或刷写记录，免费开源与Chrome刷写也只是帖中说法。未执行目标或安装依赖，REA未提，保留unverified；Fable5.2只是转述者展望，不是已使用模型。

11月24日04:00:02，Kunal（@kunal_twts）的教程回复将板型具体写作Waveshare ESP32-S3-Touch-AMOLED-1.75C，建议参考Waveshare例程的引脚和启动信息，用Claude写CO5300的QSPI显示驱动、CST9217的I2C触摸驱动，避免LVGL，只重绘变化区域，并与原厂固件比较。补取确认署名与文字。这是第三方建议和starter prompt，不是PopaSpinka公开代码、已执行的固件对照或新的60fps测量；保留其方法细节，不据教程补造硬件验收。

11月25日22:39:18的新转述给出固件名HaloWatch及重要边界：它本身只是demo，没有Wi-Fi、天气是样例、时钟从随机时间开始；另一个PopkaStudio编辑器才增加Wi-Fi对时与真实天气。帖子称Mac／Linux编辑器可在浏览器做表盘、天气、网络电台或番茄钟并加载，仍是同一圆屏项目的工具分工，不拆作新的逆向目标。它重述Claude两晚重写驱动、Opus5.5移植开放样例，并称影片中重新刷回原厂作对照；这些仍未观看或重跑。

新帖把板价写作39.99至41.99美元、HaloWatch称为MIT许可的免费GitHub release，并给Chrome／Edge或esptool刷写建议。本合集未取得对应仓库、release、许可证或刷写记录，不把教程当可安全刷写验证，也不把界面有天气图标当联网功能已具备。保留旧快照与第三方教程限制，未检查续航、硬件性能或编辑器输出。

11月22日候选封存25赞、882浏览、2转发、4回复；不是性能或续航验证。
11月24日教程回复封存0赞、15浏览、0转发、0回复；驱动型号与60fps目标来自提示，不是实测。
11月25日新候选封存0赞、43浏览、0转发、2回复；HaloWatch与PopkaStudio功能、价格及许可均为转述，未核源码或release。

## 来源

- [RetroChainer转述PopaSpinka圆屏驱动与Wear OS样例，2026-11-22 02:16:34北京时间](https://x.com/i/status/2124205345606103149)
- [Kunal的板型、显示／触摸驱动与原厂对照教程建议，2026-11-24 04:00:02北京时间](https://x.com/i/status/2124956158792503683)
- [新转述：HaloWatch demo限制与PopkaStudio联网功能分工，2026-11-25 22:39:18北京时间](https://x.com/i/status/2125600218129252514)

[English](en/popaspinka-esp32s3-wearos-ui-claude-report.md) | [返回目录](../README.zh-CN.md)
