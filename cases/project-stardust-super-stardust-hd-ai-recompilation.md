# Project Stardust：Super Stardust HD的AI辅助PS3到PC静态重编译alpha

分类：游戏与游戏保存 · 未确认使用 REA
记录日期：2026-11-25
阶段：进行中

2026年11月25日15:20:05（北京时间），The Gaming Emporium（@TheEmporium83）介绍thelastant的Project Stardust v0.1.0-alpha.2，将Housemarque于2007年推出的PS3双摇杆射击游戏Super Stardust HD静态重编译到PC。帖子明确将研究归于AI辅助、IDA Pro、MCP工具与Reverse Engineering Assistant；该英文名称不足以确定就是morluto/rea，保留rea=unknown，不猜模型。

帖子描述将原PS3 PowerPC与SPU指令转为原生C，自定义Vulkan运行时实现游戏所需图形与系统服务，Windows构建器验证游戏文件、下载依赖并生成exe。另列GameInput手柄／键盘、F1设置、持久配置、着色器缓存、独立存档目录、桌面快捷方式与原作封面整合，以及实验性Apple Silicon macOS构建流程。这些是转述的功能清单，未读取源码或发布说明，不能视作本合集测试通过。

来源明确非常早期：开发时已进入游玩，但约三分钟后冻结尚未解决，完整通关与图形准确性未验证。要求自备欧洲版NPEA00014、游戏6.00与PS3固件4.93；称当前发布物仅源码和构建工具，不含游戏。没有获取游戏、固件、发布包或依赖，也未运行构建器或目标代码。所有兼容性与发布范围均为该帖报告，不认证无资产分发或所有平台可用；按进行中项目收录，保留具体冻结限制。

封存1赞、33浏览、0转发、0回复；约三分钟冻结与功能清单均为二手项目报告。

## 来源

- [The Gaming Emporium介绍thelastant的Project Stardust alpha与冻结边界，2026-11-25 15:20:05北京时间](https://x.com/i/status/2125489687976374391)

[English](en/project-stardust-super-stardust-hd-ai-recompilation.md) | [返回目录](../README.zh-CN.md)
