# 荣誉勋章欧洲战役：Claude辅助Xbox静态重编译，作者自测Windows移植

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-01
阶段：进行中

2026年11月1日07:32:17（北京时间），The Gaming Emporium报道boodyandmustafa-create的Medal of Honor: European Assault Windows移植。原作是2005年主机二战射击游戏。补读项目固定提交d097881e242b2925589c3e6281dd88e1052bd602的README、PROJECT_STORY.md与SOURCE.txt；提交日期为10月31日16:16:33 UTC，即北京时间11月1日00:16:33，早于本窗口，属于补充一手资料。文档称Claude Code互动完成大部分逆向和编码，人类作者在真实游戏里逐次测试；不是AI无人监督的全自动移植。

项目用xboxrecomp把USA／NTSC-U的DEFAULT.XBE逐函数转C，再编译为x86-64，不再仿真Xbox CPU；但音视频芯片、内存布局等仍复用xemu派生的硬件仿真。开发故事称先从约1.3fps软件渲染优化到25～30fps，再将绘制命令转Direct3D11。鼠标支持需找到摇杆到镜头的实际逻辑；视场扩大需同步裁剪／LOD，而非只改一个数。音频研究报告逐段、逐字节比较参考解码，发现8位乘法被翻译成更宽运算造成查表错误，另修六声道到双声道混音并为长时音频缓冲停滞加恢复守卫。以上是项目过程自述，不是这里的性能或差分测试。

README标0.9.0-beta、Windows10／11 64位，提供宽屏、4K、原生鼠标、可改键、启动器和部分阿语支持。英文限制表称60／90fps稳定，120～240fps实验性；同文件阿语简述只确认60fps，不将90fps视为全语言一致的保证。长时声音仍可能中断，武器Mod只确认弹匣容量，声音替换未端到端测试，阿语字幕有缺译与裁切。

SOURCE明确重编译游戏与主体移植代码不开源，仅列xemu派生部分及重链接申请途径，不能把公开GitHub文档当作完整开源重建。文档要求自备USA游戏文件并声称不附游戏资产，本合集未下载发布包核验；个人非商用许可也不等于获得EA游戏再分发许可。未安装工具、运行游戏或独立重跑测试，REA未提及。

候选快照2赞、162浏览、1转发；本合集只读文档，未运行移植。
固定资料早于本窗口；性能、音频修复与稳定性为项目自述，主体代码非开源。

## 来源

- [The Gaming Emporium的MOH移植报道，2026-11-01](https://x.com/i/status/2116674651480809567)
- [补充窗口前固定README：AI归因、功能与限制](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/README.md)
- [补充固定开发故事：人工测试、渲染与音频诊断](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/PROJECT_STORY.md)
- [补充固定SOURCE声明：仅部分源码，主体不开源](https://github.com/boodyandmustafa-create/MOH-EuropeanAssault-PC-Port/blob/d097881e242b2925589c3e6281dd88e1052bd602/SOURCE.txt)

[English](en/moh-european-assault-xbox-claude-pc-port.md) | [返回目录](../README.zh-CN.md)
