# 死亡之屋ReWrithe：Claude辅助合并街机与PC逻辑，项目测试不等于全平台实测

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-02
阶段：进行中

2026年11月2日18:14:38（北京时间），候选介绍TawhidI-602（Tawhid）的The House of the Dead: ReWrithe，将SEGA 1996街机与1998 PC版合成C++重写，宣传宽屏、四人合作、手柄与光枪，以及Windows／Linux／Steam Deck／macOS构建。目标是保存并在现代设备运行原作，须自备Revision A街机ROM和1998 PC文件。

补读公开README，固定提交081fe6a651dbc4c43779f5ced65e705f853466ab，时间2026-11-01T16:23:10Z，即北京时间11月2日00:23:10，早于本候选。项目明确Claude协助逆向、重写和合并已有代码，由作者指挥和测试，译文也是机器生成；不声称AI生成游戏美术。v1.0.0仍是首发，许多无捕获对照的例程标UNVERIFIED，已列45项，PC序章和路线图walker仍部分实现。

README自报街机四章、最终Boss与结局的一／二人MAME回放逐帧零差异，PC Mode第一章17289帧相同及321个THOTD.EXE例程无差异；这些是项目自动对照，不是本合集重跑。人类在2026-10-21用Surface Pro 7通关街机主线。测试矩阵明确联网只在一台PC跑多份实例，尚未实测两台真机或互联网；光枪和多种手柄只做模拟输入。Linux是WSL无头测试，Steam Deck真机未测；macOS虽列CI构建路径，矩阵又称从未构建或运行，路线图仍未勾选，不把候选的全平台说法当兼容证明。

四人功能实验性；大部分AMD／Intel与旧显卡仍待实测，DualSense初始瞄准被评笨拙、改后手感待测，机器翻译待母语审读。保留公开实现和分层测试的阅读价值，但不据零差异数字宣布整作、全部模式或平台已等价。没有下载资产、编译或执行游戏。

候选快照0赞、225浏览、0转发；无独立重建，项目自报回放结果不能等同全游戏证明。
补充README早于候选，含2026-10-21与10-27等历史测试记录，不计作新候选。
平台支持、真实光枪、两台设备联网与macOS构建／运行均有明确证据缺口。

## 来源

- [候选：ReWrithe与Claude辅助开发介绍，2026-11-02](https://x.com/i/status/2117198692591575352)
- [补充固定README：AI分工、回放与人工／自动／未测试矩阵，2026-11-02 00:23:10北京时间](https://github.com/TawhidI-602/The-House-of-the-Dead-ReWrithe/blob/081fe6a651dbc4c43779f5ced65e705f853466ab/README.md)

[English](en/house-of-the-dead-rewrithe-claude-cpp-rewrite.md) | [返回目录](../README.zh-CN.md)
