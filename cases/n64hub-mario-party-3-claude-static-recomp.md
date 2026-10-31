# Mario Party 3：Claude辅助重编译，保留社区与首个移植的贡献归属

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：进行中

2026年10月31日12:51:40（北京时间），The Gaming Emporium（@McGroin83）报道n64hub的Mario Party三作独立移植。本条只记2000年的Mario Party 3。补读固定提交817b57711faf51ee694a132d4d6c3db70ff8ad96的完整README，提交为10月31日08:06:28北京时间，早于候选。

文档披露本仓库几乎所有代码、文档和测试由Claude Agent编写，人指导和试玩，不提交到拒绝AI代码的上游。以N64Recomp将MIPS转为C，结合N64ModernRuntime、RT64及RecompFrontend，复用mariopartyrd/marioparty3反编译符号和mario-party-engine调度。项目从初代重编译仓库起步，并明确感谢Rainchus的首个MarioParty3-Recomp指出音频微码位置和应挂接的overlay加载器；不把这些社区成果重标为AI首次发现。

README称菜单、六棋盘与小游戏在桌面和浏览器运行，窗口适配扩展棋盘相机、背景和HUD，提供显示刷新率插帧；游戏进程用每进程一线程、一次运行一个的共享调度器。文档列Windows／Linux x86-64与最多四人本地控制器分配，网页从自备ROM构建。限USA、32MiB大端.z64，不含游戏文件，代码GPL-3.0。不宣称完整兼容、跨网联机或已独立复现；本合集未下载ROM、安装依赖、运行构建或试玩，REA未提及。

报道候选快照119赞、2808浏览、11转发，属于三作共用帖子，不能当本作独立热度。

## 来源

- [The Gaming Emporium的三个独立Mario Party项目报道，2026-10-31](https://x.com/i/status/2116392641008951793)
- [补充：Mario Party 3固定README与前人贡献，2026-10-31 08:06北京时间](https://github.com/n64hub/mario-party-3-recomp/blob/817b57711faf51ee694a132d4d6c3db70ff8ad96/README.md)

[English](en/n64hub-mario-party-3-claude-static-recomp.md) | [返回目录](../README.zh-CN.md)
