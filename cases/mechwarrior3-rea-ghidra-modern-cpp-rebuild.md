# MechWarrior 3：REA／Ghidra研究后逐函数重写C++，公开现代平台重建

分类：游戏与游戏保存 · REA
记录日期：2026-11-04
阶段：进行中

2026年11月4日02:51:07（北京时间），一则介绍帖称Owen Morgan的MechWarrior 3重建发布1.0，为1999年的PC机甲游戏提供Windows、macOS与Linux原生运行、宽屏及最多八人联机。补读公开仓库README及固定提交bb9af7b22c54c909cec8052595c1fe0bb32773f1：项目明确称研究Mech3.exe 1.2，使用Ghidra与REA逐函数重写C++，借mech3ax交叉检查数据格式，并以Unicorn模拟原版作对照；不是简单静态重编译或Wine包装。固定提交时间为11月4日01:29:09北京时间，属于用于核对方法与范围的项目记录，不是另一个候选。

README描述SDL3和Direct3D 12／Metal／Vulkan后端、1.0数据按1.2行为加载、自建UDP联机取代DirectPlay，并列出原有机制与兼容修复。须自备原游戏文件，不分发游戏资产；Pirate's Moon尚不支持。候选明确说Linux AppImage已构建但未试玩，不能把三平台发布列表当三平台实测。作者所称多数逻辑经模拟器对照没有在此重跑，不据此声称全游戏字节匹配、战役通关或跨平台联机已独立验收。未下载发行包、安装依赖、构建或运行游戏。

候选快照11赞、410浏览、1转发；Linux未试玩和扩展未支持的边界保留。

## 来源

- [MechWarrior 3现代重建介绍，2026-11-04](https://x.com/i/status/2117691059149115770)
- [固定项目README：REA／Ghidra署名、方法与兼容范围，提交于2026-11-04北京时间](https://github.com/telltaleatheist/mw3-re/blob/bb9af7b22c54c909cec8052595c1fe0bb32773f1/README.md)

[English](en/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md) | [返回目录](../README.zh-CN.md)
