# Mario Party初代：n64hub以Claude辅助静态重编译到桌面与浏览器

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：进行中

2026年10月31日12:51:40（北京时间），The Gaming Emporium（@McGroin83）报道n64hub的Mario Party三部曲，但明确是三个独立项目。本条只记录1998年初代Mario Party。补读固定提交ac7f9b52fc07ecbf20b180ef4854563e2d0c610b的完整README，提交为10月31日08:06:58北京时间，早于候选；另两作分别收录。

项目将原N64 MIPS代码经N64Recomp转为C原生运行，配N64ModernRuntime、RT64和RecompFrontend，复用mariopartyrd/marioparty的社区反编译符号，不是Claude从零恢复全部游戏代码。README明确本仓库几乎所有代码、文档和测试由Claude Agent编写，人指导和试玩，不把这些代码提交给不接受AI代码的上游。共享mario-party-engine调度器以每进程一个线程、一次只运行一个来处理游戏setjmp／longjmp式进程切换，桌面与浏览器复用这部分。

项目称棋盘与小游戏可运行，RT64扩展棋盘视野、背景和HUD并做显示刷新率插帧，浏览器页面由用户ROM生成；文档列Windows和Linux x86-64发行路径及最多四名本地玩家的控制器分配。只支持USA、32MiB大端.z64，不含ROM与游戏资产。未下载ROM、依赖或发行包，未构建、试玩或验证网页与兼容性；可玩与平台覆盖仍为项目自述，不表示每个小游戏完整通过。本仓库代码GPL-3.0，原游戏与上游保留各自权利。

报道候选快照119赞、2808浏览、11转发，属于三作共用帖子，不能当每作独立热度。

## 来源

- [The Gaming Emporium的三个独立Mario Party移植报道，2026-10-31](https://x.com/i/status/2116392641008951793)
- [补充：初代Mario Party固定README，2026-10-31 08:06北京时间](https://github.com/n64hub/mario-party-recomp/blob/ac7f9b52fc07ecbf20b180ef4854563e2d0c610b/README.md)

[English](en/n64hub-mario-party-claude-static-recomp.md) | [返回目录](../README.zh-CN.md)
