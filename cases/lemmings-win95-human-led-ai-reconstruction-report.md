# Lemmings for Windows 95：人类定架构，REA与多Agent辅助的696函数重建

分类：游戏与游戏保存 · REA
记录日期：2026-11-12
阶段：进行中

2026年11月12日16:30:18（北京时间），yibie（@yibie）介绍Lemmings for Windows 95项目，强调人类负责架构与验证、AI辅助研究，不将整个旧游戏自动归功于模型。补查NitrosGits/Lemmings-For-Windows-95的固定README，提交ad29aa806811dca6cb3716a4f167ad52f6043ac6于11月9日17:37:56北京时间，早于候选。目标是Visual Sciences制作、Psygnosis于1995年发行的Windows版旅鼠，以源代码重建保存游戏并适配现代Windows及Wine。

文档列Ghidra作控制流、类型和初始伪代码研究，Hopper与REA检查基本块、控制流图与全局引用；Google Antigravity、Claude和Codex CLI在人类指导下分析x86、把伪代码转成C／C++、提出Pentium调度与寄存器分配假设、设计Python搜索。验证路线使用原Microsoft Visual C++2.2的/Ox编译、逐函数字节对照和全局内存布局检查，另以llvm-mingw／GCC及自带精简CRT构建32位Windows可移植目标。

固定文档自报一个EXE和七个DLL共696／696函数匹配，覆盖界面、文件、关卡、位图、内存、渲染和旅鼠物理／技能逻辑；它同时明确所谓byte-identical是函数编译代码，不是整个EXE／DLL文件。头、导入表与部分重定位地址仍有差异，不能标题化成全部原二进制已恢复。文档另称Windows11 ARM64虚拟机及Windows CI构建通过，但研究搜索、调试与玩法harness仍限macOS／Linux；没有本合集重跑。

必须自备合法原版游戏资产与匹配编译器，文档称仓库不含图像、音乐、关卡等资产。这里只静态阅读README，未核全部源文件、AI会话、逐函数结果或完整通关，也未构建或运行原游戏；100%函数匹配不证明一切可移植行为或整文件一致，保留进行中与项目自测归因。

候选整帖封存3赞、275浏览、0转发、1回复；696函数及构建结果为固定项目文档自报，不是独立复现。

## 来源

- [yibie的三个游戏AI研究项目介绍，2026-11-12 16:30:18北京时间](https://x.com/i/status/2120796315898777815)
- [补充固定Lemmings README，2026-11-09 17:37:56北京时间提交，早于候选；方法、状态与限制](https://github.com/NitrosGits/Lemmings-For-Windows-95/blob/ad29aa806811dca6cb3716a4f167ad52f6043ac6/README.md)

[English](en/lemmings-win95-human-led-ai-reconstruction-report.md) | [返回目录](../README.zh-CN.md)
