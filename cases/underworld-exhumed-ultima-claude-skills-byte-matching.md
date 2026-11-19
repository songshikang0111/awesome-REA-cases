# Underworld Exhumed：Exhume的Claude Code技能辅助重建两部Ultima Underworld

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-20
阶段：待验证

2026年11月20日00:34:04（北京时间），The Ultima Codex介绍两部Ultima Underworld的字节匹配反编译与Windows、macOS、Linux、浏览器移植。按具名项目补查abedegno的Underworld Exhumed，目标是保存1992年The Stygian Abyss和1993年Labyrinth of Worlds的DOS行为。同一仓库两作作为一个保存项目，不与Borland编译器案例合并。

补读11月17日UTC提交54ffea7的项目README及固定版本Exhume README。Exhume明确为Claude Code技能与编译、逐函数匹配、链接比较、录制回放和模糊测试工具，称起源于UW2；这支持AI辅助工作流，不代表AI独自完成项目。项目报告用原Borland工具得到整文件字节一致的UW.EXE／UW2.EXE；同源移植以17／13段DOS录制会话检查macOS、Linux、Windows与Node.js下Web构建。较早Exhume快照会话数不同，不当成独立测量相加。

项目列UW1的89个C文件、50个汇编模块，UW2的99个C文件及汇编，发布版本分别1.0.3和1.2.4。以上是项目报告，未审完整验证日志、运行CI、编译或游玩；字节一致也不证明唯一恢复原始源码。原生版需自备合法游戏数据，原创工具许可不授权衍生游戏代码与资产，未打开另行托管的游戏Web页。补充文档早于候选窗口，REA未确认，保持unverified。

候选封存45赞、579浏览、3转发、1回复，不代表独立验证。

## 来源

- [The Ultima Codex介绍双作反编译与移植，2026-11-20](https://x.com/i/status/2123454774721101948)
- [补充：固定11月17日UTC提交的项目README](https://github.com/abedegno/underworld-exhumed/blob/54ffea7c08d562176a8edf7398a6ff3fd372a9d2/README.md)
- [补充：固定Exhume README，Claude Code技能与UW2起源](https://github.com/abedegno/Exhume/blob/160202277647e7e97cca8a06e76184f88c573748/README.md)

[English](en/underworld-exhumed-ultima-claude-skills-byte-matching.md) | [返回目录](../README.zh-CN.md)
