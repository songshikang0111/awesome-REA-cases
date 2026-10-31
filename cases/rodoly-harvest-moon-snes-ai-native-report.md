# SNES牧场物语：RodoLy借AI逐例程恢复C，公开原生PC beta

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：分析测试

2026年10月31日12:48:40（北京时间），The Gaming Emporium（@McGroin83）报道RodoLy的1996年SNES《牧场物语》C重建与PC beta，称778个例程、45176条指令完成验证，AI使用为暂定重度、人工监督。它不是既有PS1《Back to Nature》案例。

补读RodoLy/HarvestMoonSnesDecomp固定提交54e7371118af81ba6c9a8b00dbd6b951a7d43099的完整README；提交为10月30日07:50:50北京时间，早于候选。作者称喜欢原作，完成重编译后希望逐例程理解并让游戏只运行恢复的C。明确承认AI协助，由人指导、在自己PC测试并决定保留内容，未指明模型或REA。基于ElisaS-Codes与DasK的HM-Decomp命名和内存图；项目统计100%指令／例程覆盖，测试要求128KB WRAM（含栈）、CPU与DMA寄存器相同，另有随机调用和脚本游玩检查。此处是项目文档，不是本合集重跑或覆盖全部游戏状态的证明。

原生构建直接调用恢复的C，不做SNES CPU模拟，但仍软件实现画面与声音芯片。文档说明Windows x64／ARM64与Linux路径，Windows beta下载为源码和本机构建脚本，不是即开即玩的完整游戏包。须自备合法USA ROM；公开可选16:9、十槽状态保存、HM64式暂停菜单、第三年结局后继续经营等。宽屏在地图边缘、小房间和标题回到4:3，不能称全场景宽屏。项目代码采用PolyForm Noncommercial，不授权原游戏资产。未下载ROM、安装依赖、构建游戏或执行校验，保留beta与项目自测边界。

候选快照0赞、194浏览、0转发；778与45176及100%均为项目口径，未独立验证。

## 来源

- [The Gaming Emporium的SNES牧场物语报道，2026-10-31](https://x.com/i/status/2116391886118121955)
- [补充：固定README的AI披露、验证方法和原生构建，2026-10-30](https://github.com/RodoLy/HarvestMoonSnesDecomp/blob/54e7371118af81ba6c9a8b00dbd6b951a7d43099/README.md)

[English](en/rodoly-harvest-moon-snes-ai-native-report.md) | [返回目录](../README.zh-CN.md)
