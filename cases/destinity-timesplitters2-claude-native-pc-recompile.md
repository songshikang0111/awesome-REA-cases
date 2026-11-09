# TimeSplitters 2：Destinity与Claude重编译PS2版，按PCSX2追查差异

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-10
阶段：进行中

2026年11月10日01:43:29（北京时间），Destinity（@blackintrax）称与Claude共同制作TimeSplitters 2原生PC版：自己试玩与决策，AI承担大量逆向，每个修复逐帧对照PCSX2，工具代码GPL-3.0。补取同串01:43:24与01:43:28，作者报告PS2代码重编译为x86、60FPS、真实16:9与最高4K，Linux／Steam Deck可玩，Windows与在线联机待发布；启动器在用户电脑从自有光盘镜像构建，约三分钟是作者估计。

补读Destinity13/TimeSplitters-2-Native-Linux-Recomp的README、VERIFICATION与KNOWN_ISSUES，固定提交55722bd4e41937a6dac8c81dcd2fea821412caee（11月9日18:06:01北京时间，早于本窗口）。路径是PS2Recomp派生的R5900 MIPS到C++、VU1到C++／SSE，再编译本机可执行文件；不是运行时CPU模拟，但仍使用PCSX2 GS与SPU2提供图形／声音，部分内核、I/O和时序由运行时高层实现。不能把“原生”写成完全不依赖模拟器组件。文档披露Claude参与逆向、实现、测量与文档，人工控制方向、硬件与试玩。

验证文档说明以输入回放、截图、savestate寄存器、RAM、日志寻找首个差异，称参考路线1090万次VU1调用的寄存器与GS输出一致；但开头明确内部测试／参考工具未公开，无法据此重放全部检查。已知问题文档另保留0x18d8程序尾CLIP寄存器因约90周期时序差而不一致、称暂不影响画面，不能把路线结果泛化为所有状态位完全相等。

项目自报首关Siberia在PC／Deck及双人合作通关，Arcade League、Challenge、MapMaker等可用；第2至10关、Arcade Custom与三四人仍待测。部分角色预览菜单49至56FPS，主菜单／游戏约59.9FPS；音频修复仍在试玩确认。Windows与最多16人的在线模式虽文档称已构建，仍标1.0待发布，互联网联机待测，不能写已全面上线或全游戏通关。需要自备USA SLUS-203.14光盘；源码许可不授权原游戏。未下载游戏、构建、运行测试工具或试玩，以上是公开项目记录，不是本合集独立复现；REA未提及。

候选封存0赞、11浏览、0转发；补取同串用于定位项目，不替换候选。
固定提交2026-11-09T10:06:01Z；60FPS、4K、1090万次与三分钟均为项目值，未独立重跑。

## 来源

- [候选：Destinity披露Claude逆向、人工试玩与PCSX2对照，2026-11-10](https://x.com/i/status/2119848363772248275)
- [补充同串：TimeSplitters 2原生PC版与平台阶段，2026-11-10 01:43:24北京时间](https://x.com/i/status/2119848340917797362)
- [补充同串：从自有光盘本机构建，2026-11-10 01:43:28北京时间](https://x.com/i/status/2119848361423520203)
- [窗口前固定README：架构、状态与AI披露，2026-11-09提交](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/README.md)
- [同提交验证文档：内部工具未公开、VU1路线比较](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/docs/VERIFICATION.md)
- [同提交已知问题：11月8日v0.9.9记录与未测范围](https://github.com/Destinity13/TimeSplitters-2-Native-Linux-Recomp/blob/55722bd4e41937a6dac8c81dcd2fea821412caee/docs/KNOWN_ISSUES.md)

[English](en/destinity-timesplitters2-claude-native-pc-recompile.md) | [返回目录](../README.zh-CN.md)
