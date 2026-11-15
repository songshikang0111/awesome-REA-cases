# PocketPort Anything：AI辅助3DS移植研究框架，不是任意游戏转换器

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-15
阶段：进行中

2026年11月15日16:30:12（北京时间），yibie（@yibie）的列表更新介绍PocketPort Anything，强调anything只是调查范围，不承诺兼容性。同帖的The Console skill已在本合集收录；本项目是另一套面向Nintendo3DS的AI辅助研究与工程框架，不是PS2工具的改名，也不把同帖其他目录作为新游戏成果。

通过列表定位Alexispher/pocketport-anything，补读固定9a7d588a2574683ca33f9c4717d472193916f986 README，提交为2026年11月15日02:17:03 UTC，早于窗口。文档让Claude Code、Codex等Agent先识别引擎、格式和已有源码移植，再选择重建、适配或明确标注的替代路线，保存构建和验证证据。其实际范围包括文件清单、只读NUP元数据、有限uint32中间表示到C99与主机语义对照，以及原创新游戏Star Catcher的C运行时；不是ARM64、x86或MIPS通用机器码翻译器。

文档自报Star Catcher双屏及有限Skyrim3D查看器已交叉编译，但同构建双屏像素、Azahar和物理3DS仍未验证。Skyrim路径只有受限BSA／TES5／NIF静态资源和几何研究，不含完整世界、碰撞或原游戏玩法；后加源码工程流水线提及The Legend of Edgar和L'Abbaye des Morts源码调查，也不等于完整3DS可玩。README部分旧roadmap与后附实现更新并存，不能把所有待办都说成已实现，亦不把主机测试当实机证明。

项目称MIT，不分发商业游戏数据；NUP在此是模拟器特定容器，文件扩展名不证明官方包或3DS兼容。v0.3.1归档与部分0.2.0包元数据不同，按文档保留而不替作者修正。REA仅在研究参考中出现，不证明该框架执行时用了REA。本合集未安装依赖、执行目标、构建或重跑项目测试，按进行中研究框架收录。

候选整帖8赞、533浏览、0转发、7回复；不是本项目单独热度。
v0.3.1与0.2.0是文档说明的版本口径差异；没有已验证的完整商业游戏移植数。

## 来源

- [yibie介绍PocketPort与TA Reborn等，2026-11-15 16:30:12北京时间](https://x.com/i/status/2121883453767688434)
- [窗口前固定PocketPort README：方法、实现与未验证范围，提交2026-11-15 02:17:03 UTC](https://github.com/Alexispher/pocketport-anything/blob/9a7d588a2574683ca33f9c4717d472193916f986/README.md)

[English](en/pocketport-anything-ai-3ds-porting-research-framework.md) | [返回目录](../README.zh-CN.md)
