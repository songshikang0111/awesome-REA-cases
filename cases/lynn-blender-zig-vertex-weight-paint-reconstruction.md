# Blender局部重建：Lynn尝试抽取顶点创建、整合与权重绘制

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-20
阶段：进行中

2026年11月20日01:52:37（北京时间），Lynn Cole（@priestessofdada）将Blender中负责顶点创建、consolidation（整合）与权重绘制的部分列为第三个测试。Blender是3D创作套件；目标是把需要的局部功能重建成可复用Zig应用或库，而不是保留多年累积的整个产品。

作者称新工具由未具名Rust重建应用变为Zig，与Agent配合测量输出和推断行为，允许功能变体。没有Blender版本、输入模型、数据结构、误差标准、Zig代码或绘制对照，且她说这些测试尚未完成。不能把consolidation擅自限定为某种焊接算法，也不能宣称完整Blender兼容。

补读Blender README只确认公开3D套件及整体GPLv3许可背景，不验证作者的实现或clean-room合法性，公开代码不等于本次直接移植。该背景于11月20日阅读，未固定版本、原始发布日期未确定。REA未提，Agent型号未知，未运行Blender或重建代码；同帖其他目标分列。

## 来源

- [Lynn的Blender局部重建测试，2026-11-20](https://x.com/i/status/2123474539669573873)
- [补充背景：Blender README与许可说明，未固定版本](https://github.com/blender/blender)

[English](en/lynn-blender-zig-vertex-weight-paint-reconstruction.md) | [返回目录](../README.zh-CN.md)
