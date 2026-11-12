# Tony Hawk's Underground：AI可逐函数贡献，合并靠确定性门禁而非AI

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-12
阶段：进行中

2026年11月12日16:30:18（北京时间），yibie（@yibie）介绍andrewnakas/thug-decomp，称贡献入口同时面向人和AI，但合并环节不用AI。补读固定提交dba7457cf8ea3bad7af718db46c2876863e1f36b的README和START_HERE，提交于11月7日12:09:30北京时间，早于候选。目标为Neversoft／Activision2003年PS2游戏Tony Hawk's Underground的NTSC-U版SLUS-20731，逐函数重建可匹配的C++，用于保存与研究。

文档列SN Systems ee-gcc2.95.3、SN BUILD1.36和splat／spimdisasm拆分的11438个函数。全ELF由C++加汇编重建可字节一致，不能据此宣称11438个函数都已转成C++；当前C++完成比例交给动态进度站，本合集未取该比例。候选的9252文件是清单作者口径，不是匹配函数数，也未核树文件总量。

START_HERE提供给Agent的任务协议：先读规则，不接触泄漏源码，自备光盘，认领未占地址，逐函数生成草稿、比较、修正，再开至多20函数的PR。首次PR需维护者judge-ok标签，之后由本地Decompathon Steward自动判断和合并，因此不用AI不等于每次纯人工点合并。README列五道确定性门禁：固定工具链校验、禁止内联汇编等投机形式的扫描、拆分完整性、指令匹配、整ELF哈希和objdiff对照；公共CI仅做不需要光盘的检查。

它展示Agent参与受限的具体协作设计，不是云模型凭空生成整款游戏或无审查接纳代码。只静态阅读文档，没有审实际PR、Steward实现、AI执行日志或运行门禁，也未获取光盘、编译器或游戏文件。REA未见提及；保留进行中与项目自报匹配边界。

候选整帖封存3赞、275浏览、0转发、1回复；9252文件为候选说法，不是完成度。没有独立构建结果。

## 来源

- [yibie的THUG人类／AI贡献与非AI合并介绍，2026-11-12 16:30:18北京时间](https://x.com/i/status/2120796315898777815)
- [补充固定THUG README，2026-11-07 12:09:30北京时间提交，早于候选](https://github.com/andrewnakas/thug-decomp/blob/dba7457cf8ea3bad7af718db46c2876863e1f36b/README.md)
- [同一固定提交START_HERE：自备光盘、Agent贡献与首PR审批流程](https://github.com/andrewnakas/thug-decomp/blob/dba7457cf8ea3bad7af718db46c2876863e1f36b/START_HERE.md)

[English](en/tony-hawks-underground-agent-contribution-report.md) | [返回目录](../README.zh-CN.md)
