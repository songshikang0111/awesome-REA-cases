# decompdecomp：续接decomp.wtf的独立工作台，字节匹配不等于全游戏已恢复

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-14
阶段：进行中

2026年11月14日00:50:08（北京时间），Pixel Cherry Ninja（@PixelCNinja）介绍decompdecomp，让Claude、Codex、Cursor为自有游戏恢复可字节匹配的C／C++，称N64就绪、GBA／PS1／GameCube／DS为beta且完全本地。补查公开仓库定位到n-delic/decompdecomp，读取README，固定到9e19b4d79f8798df626e6216385ac91b3642535d；提交于11月13日07:47:52北京时间，早于本候选窗口，是补充背景，不是本轮新测试。

文档描述原游戏编译器编译Agent输出，仅字节相同才算函数匹配，多Agent可并行处理函数，自动流程先处理容易函数。关键限制是“尚无整款游戏已反编译”：导出混合已匹配C和其余汇编，因此能重建不等于全C恢复。N64标Recommended，多种其他主机／PC平台标Beta，部分只接公开社区反编译；Windows的PS1、PS2和多数N64需要WSL2，macOS另有编译器限制。平台表和导出能力均为项目文档口径，不是本合集实跑验收。

README明确继续Sam Wolfs的decomp.wtf代码，原项目做到0.10.6后归档；同时说明独立维护、与原作者无关联且没有其背书。因此单列这个后续项目，保留旧Decompwtf条目，不把旧停更消息当成新项目也停更。新代码AGPLv3，原MIT通知另存；项目要求自备有权使用的游戏、不发布恢复的游戏代码。其隐私说明有重要例外：材料除发送给所选模型外留在电脑上，故不能把“完全本地”理解成云模型绝不收到游戏内容。未安装、导入ROM、构建、运行测试或独立检查字节匹配日志，未确认REA；按进行中项目收录。

候选快照16赞、1129浏览、0转发、3回复；没有整款游戏完成、平台和隐私例外来自项目文档，未复跑。

## 来源

- [Pixel Cherry Ninja介绍decompdecomp，2026-11-14 00:50:08北京时间](https://x.com/i/status/2121284490500981068)
- [窗口前补充：项目README固定于11月13日07:47:52北京时间提交，后续取阅](https://github.com/n-delic/decompdecomp/blob/9e19b4d79f8798df626e6216385ac91b3642535d/README.md)

[English](en/decompdecomp-local-agent-byte-matching-workbench.md) | [返回目录](../README.zh-CN.md)
