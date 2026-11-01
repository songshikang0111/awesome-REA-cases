# PE2PC：Snaity以Claude辅助把寄生前夜II既有反编译移植到Windows

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-02
阶段：进行中

2026年11月2日02:12:46（北京时间），候选报道Snaity（Adriano Teodoro）的PE2PC，把Square的1999年PlayStation游戏《寄生前夜II》移植到Windows，建立在GabeRealB及贡献者的既有反编译上，而不是Claude从零独自恢复全游戏。

补充公开检索找到Snaity-CORE/pe2-pc-port，阅读固定f8b34d128694f950e0c827b898d163621be2ccc3的README，提交时间2026-11-01T07:54:36Z（北京时间11月1日15:54:36），早于候选。文档说明把反编译C编译为PC原生代码，以自有C兼容层和Rust host替代图形、声音、CD、控制器、记忆卡等主机服务；自述无需模拟器、无Sony代码。Claude Code编写大量代码、工具和文档，Snaity设目标、审改动、游玩测试、用DuckStation比较并提交；AI贡献不能覆盖成反编译作者署名。

项目报告Windows双盘、影音、存档与控制器可用，最高8倍原320×240分辨率、亚像素顶点与透视正确纹理；游戏仍30fps运行，以模型中间帧呈现60fps。支持相机相对移动、可改键、滤镜、高清文字和实验性替换素材／翻译等Mod，原始.mcd记忆卡可与DuckStation互通。这些是项目功能与测试自述，不是本合集通关、性能或延迟实测；nightly明确仅经CI。

须自备美版SLUS-01042与SLUS-01055光盘的CHD／CUE镜像，Windows10／11与Vulkan或OpenGL3.3；仓库称不含游戏数据。原创代码CC0不授权Square资产，字体和库另有许可。只静态阅读，未下载发行包、资产、安装依赖、构建或运行游戏；未提REA。

候选快照50赞、1004浏览、12转发；项目README日期早于候选，不算本轮另一个帖子。
60fps为30fps游戏逻辑间插帧；未独立重建或验证双盘通关，nightly仅经CI。

## 来源

- [候选：PE2PC移植与Claude分工报道，2026-11-02](https://x.com/i/status/2116956628771873001)
- [补充固定README：原生架构、AI分工与测试边界，2026-11-01](https://github.com/Snaity-CORE/pe2-pc-port/blob/f8b34d128694f950e0c827b898d163621be2ccc3/README.md)

[English](en/parasite-eve2-pe2pc-claude-native-port.md) | [返回目录](../README.zh-CN.md)
