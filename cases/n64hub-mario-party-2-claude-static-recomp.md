# Mario Party 2：n64hub的Claude辅助原生与网页重编译项目

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：进行中

2026年10月31日12:51:40（北京时间），The Gaming Emporium（@McGroin83）报道n64hub的三个独立Mario Party静态重编译项目。本条是1999年的Mario Party 2，不是初代附加模式。补读固定提交bd4ee2d474d6ca4cffe178669549300880b59659的完整README，提交为10月31日08:07:23北京时间，早于候选。

README明确本仓库几乎所有代码、文档和测试由Claude Agent编写，由人指导和试玩，不向不接受AI代码的上游提交。技术路径为N64Recomp将游戏MIPS转C，以N64ModernRuntime、RT64及RecompFrontend原生执行和呈现，复用mariopartyrd/marioparty2反编译符号及mario-party-engine共享进程调度器；社区原有研究不能归为本作者或AI独立完成。

文档称菜单、六张棋盘与小游戏可在桌面和浏览器运行，棋盘视角、背景、玩家面板适配窗口形状并插帧到显示刷新率；共享调度器每个游戏进程独立线程、一次运行一个。浏览器需从自己的ROM构建页面；提供Windows／Linux x86-64发行路径及最多四人本地控制器分配，只支持USA、32MiB大端.z64。仓库不含ROM或游戏资产，代码为GPL-3.0。未下载游戏或发行包、安装依赖、构建或试玩，不把README状态当全兼容验收；REA未提及。

报道候选快照119赞、2808浏览、11转发，为三作共用帖子，不是本作单独热度。

## 来源

- [The Gaming Emporium的三作独立移植报道，2026-10-31](https://x.com/i/status/2116392641008951793)
- [补充：Mario Party 2固定README，2026-10-31 08:07北京时间](https://github.com/n64hub/mario-party-2-recomp/blob/bd4ee2d474d6ca4cffe178669549300880b59659/README.md)

[English](en/n64hub-mario-party-2-claude-static-recomp.md) | [返回目录](../README.zh-CN.md)
