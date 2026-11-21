# ESP32-S3圆屏重建Wear OS界面：PopaSpinka的Claude驱动与样例移植转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-22
阶段：待验证

2026年11月22日02:16:34（北京时间），RetroChainer转述YouTube作者PopaSpinka的项目：40美元Waveshare ESP32-S3、466×466圆形AMOLED且无GPU，原厂滚动图标撕裂，不能手指拖动。帖子称开发者不用LVGL或Arduino_GFX，借Claude Code从头写显示、触摸驱动和绘图库，再由Opus5.5移植Google开放Wear OS样例，含滚动数字、Pixel Watch式卡片、天气和音乐界面。

两天两个晚上、60fps、零丢帧、零撕裂、静止时零绘制均为该帖转述；3:22原厂撕裂与4:16标准驱动闪烁是作者给的影片位置，未观看或测量。本项目是已有开放样例及设备行为的改造，不是破解Pixel Watch或以40美元复刻Google收购的全部技术。

补读回复，有人询问电池唤醒首帧，未见测试答复；不把少绘制自动升级为已测续航。未取得仓库、代码或刷写记录，免费开源与Chrome刷写也只是帖中说法。未执行目标或安装依赖，REA未提，保留unverified；Fable5.2只是转述者展望，不是已使用模型。

候选封存25赞、882浏览、2转发、4回复；不是性能或续航验证。

## 来源

- [RetroChainer转述PopaSpinka圆屏驱动与Wear OS样例，2026-11-22 02:16:34北京时间](https://x.com/i/status/2124205345606103149)

[English](en/popaspinka-esp32s3-wearos-ui-claude-report.md) | [返回目录](../README.zh-CN.md)
