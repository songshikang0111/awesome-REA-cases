# D2-Web：人类指导AI重建Diablo II 1.13c浏览器引擎，仍是Act1早期Alpha

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-01
阶段：进行中

2026年11月1日08:25:54（北京时间），候选报道Virtastic的D2-Web，把Diablo II: Lord of Destruction 1.13c引擎以C++20重实现并编译成WebAssembly，在Chrome／Chromium本地执行而非云串流。帖子列宽屏、手柄、七职业、共享仓库和自动存档，同时明确Act1早期Alpha，不能当作完整Diablo II。

补读固定提交2bb0efe4808065b6a7d6409300da847c6757ec91的README，提交日期为11月1日03:14:36 UTC，即北京时间11:14:36，晚于候选，作为补充一手文档。它确认大量代码由AI工具协助、人工维护者指导审查，研究零售1.13c程序且并非净室，部分代码改编自MIT许可D2MOO，并使用StormLib等前人工作。README仅明确Act1角色创建、营地、初始野外、战斗、物品、商人、传送点与存档可运行，仍有缺失画面与错误行为；候选的七职业等未逐项测试。

默认BYO模式由玩家选本机MPQ、文件留浏览器，文档另有服务器托管MPQ模式，不能笼统保证所有部署都不上传文件。开发服务器无认证，文档警告可访问者可下载所配置MPQ、不得公开分发；Wasm线程还需跨源隔离标头及HTTPS或localhost。存档按设备留浏览器，不连接Battle.net。自有源码MIT不授权分发Blizzard资产，必须有合法1.13c游戏文件。本合集仅读文档，未安装依赖、获取游戏数据、部署服务器或重跑差分／游戏测试。

候选快照17赞、1019浏览、1转发；没有独立游戏或差分测试。
补充文档晚于候选；BYO与托管文件模式隐私边界不同，早期Alpha并非完整游戏。

## 来源

- [候选：D2-Web浏览器移植与AI参与报道，2026-11-01](https://x.com/i/status/2116688145823486161)
- [补充：11月1日11:14固定README，AI归因、Alpha与部署边界](https://github.com/Virtastic/d2-web/blob/2bb0efe4808065b6a7d6409300da847c6757ec91/README.md)

[English](en/d2-web-diablo2-ai-wasm-reimplementation.md) | [返回目录](../README.zh-CN.md)
