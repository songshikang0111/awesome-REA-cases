# Project Avalanche：Claude辅助研究SSX 2012光盘与行为，以Rust／Bevy重建PC版

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-09
阶段：进行中

2026年11月9日06:34:13（北京时间），The Gaming Emporium（@McGroin83）介绍MnkyArts的Project Avalanche：将EA的Xbox 360滑雪游戏SSX（2012）带到现代PC，研究原盘数据与游戏行为，再以Rust和Bevy独立重实现，不是运行Xbox 360模拟器或静态重编译。补查公开项目README，固定到208af62913ea8b8f3f32a9530123783516aa83cc（11月9日00:14:15北京时间）后确认文本与读取版本一致。此项目记录早于候选、在本窗口之外，只作补充证据，不冒充新的候选帖子。

项目明确写明Claude辅助开发，原始格式来自维护者自有零售光盘、行为来自游戏代码。致谢列出Ghidra经GhidraMCP供工具研究，以及ImHex、Kaitai Struct等结构分析工具；未见REA使用声明。文档称已在单窗口接入开场影片、菜单、新建档案、World Tour／Explore、滑雪物理、HUD、音乐语音音效、比赛结果与保存进度。启动器从用户自有Xbox 360 ISO提取约4.7 GB数据，另有Windows／Linux构建、专用服务器、公网列表及LAN发现，支持Luau脚本、地图和模式Mod；这些是项目描述，不是本合集实跑结果。自动更新说明保留存档与数据，不据此保证升级无风险。

项目称尽可能对零售盘核验，包括解析器的全盘验证、与游戏代码和参考解码器对照，但没有人完整通关；尚未解码的行为以TODO(guess)标注近似和待解决的地址或问题。构建及CI命令只是文档，不是本合集执行日志；不宣称全流程可玩、原版物理等价、联机稳定或所有机器兼容。Linux文档要求Vulkan、ALSA及Wayland／X11，构建基于Ubuntu 24.04 x86-64及相应或更新glibc，不等于任意Linux均支持。

自有代码标MIT，原SSX及光盘内容仍属EA；项目说仓库与构建不含游戏数据，用户须自备合法取得的兼容零售盘镜像。本合集只读取原帖、公开元数据和固定README，未下载发行包、游戏资产、执行目标代码、构建或试玩；项目自述核验不等于独立复现。

候选封存快照4赞、327浏览、1转发；补取原帖浏览数已变化，保留封存值。约4.7 GB为项目提取数据规模，非重建源码规模或正确率。

## 来源

- [The Gaming Emporium的Project Avalanche介绍，2026-11-09 06:34:13北京时间](https://x.com/i/status/2119559143551799341)
- [补充项目README：固定2026-11-09 00:14:15北京时间提交，含AI归因与未通关边界](https://github.com/MnkyArts/ProjectAvalanche/blob/208af62913ea8b8f3f32a9530123783516aa83cc/README.md)

[English](en/project-avalanche-ssx2012-claude-bevy-reimplementation.md) | [返回目录](../README.zh-CN.md)
