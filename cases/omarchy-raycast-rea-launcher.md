# oma-launcher／oma-cast：REA 研究 Raycast 后为 Omarchy 重建启动器

分类：应用与客户端 · REA
记录日期：2026-10-31
阶段：进行中

10月20日03:34（北京时间），@typecraft_dev称数小时用REA做出Omarchy的Raycast式启动器，支持习惯排序、应用及Omarchy动作统一搜索、别名收藏、键盘操作和实时主题，约40ms打开。此前补查typecraft-dev/oma-cast采用10月20日03:20的9375380fe04dc67fd06752d884ea8cfe9d1eabad提交，其中仍称oma-launcher；04:03后续改名不倒填为当时窗口内事实。

已读该提交README、RootSearch.js及后端研究笔记相关可读部分。项目要求Omarchy 4、Hyprland 0.56+与omarchy-shell，作为QML插件而非Electron/Node守护进程运行；代码可见应用及菜单候选、别名收藏、frecency和搜索回退。笔记明确目标为Raycast 2.8.2，区分静态观察与推断，记录REA打开原生模块时Hopper超时，部分常量改用objdump读取，不能称所有发现都由REA完成。

设置窗口、Script Commands、剪贴板历史、snippets、quicklinks、计算器、Raycast扩展、窗口管理与rayconfig导入在该固定提交仍为路线图，不是完整Raycast替代。独立clean-room及无Raycast代码资产为项目声明，非法律审核；产品无AI功能不等于开发未用AI。存在单元与smoke测试文件，但此前Actions接口未返回运行记录，本合集未运行目标测试或桌面。数小时、约400菜单动作与40ms均为作者／项目说法。

2026年10月31日23:35:10（北京时间），同一作者typecraft发布亲自制作REA及如何做出omacast的视频。补查原帖确认账号，公开链接实体展开至YouTube的uMoRUue2wzI，标题为I used the viral reverse engineering tool。此次新增可追溯的作者演示入口，不把旧项目重复计数。未播放或取得字幕，不能从视频标题推定新功能完成、差分测试通过或旧路线图已全部实现；旧固定源码证据仍保持原日期与范围。

10月20日候选106赞、1985浏览、3转发；当时补取130赞、2458浏览、3转发，非性能验证。
10月31日视频候选16赞、1208浏览、0转发；未观看视频或验证新增功能。

## 来源

- [typecraft的REA启动器发布](https://x.com/i/status/2112266105200800245)
- [窗口内固定提交README与路线图](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/README.md)
- [同提交RootSearch实现](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/plugin/core/RootSearch.js)
- [同提交Raycast静态研究与Hopper超时说明](https://github.com/typecraft-dev/oma-cast/blob/9375380fe04dc67fd06752d884ea8cfe9d1eabad/reference/02-backend.md)
- [作者REA／omacast视频发布，2026-10-31](https://x.com/i/status/2116554581580886102)
- [补充：作者视频I used the viral reverse engineering tool，未观看](https://www.youtube.com/watch?v=uMoRUue2wzI)

[English](en/omarchy-raycast-rea-launcher.md) | [返回目录](../README.zh-CN.md)
