# Pokémon Bank／Mover：Wokann公开Codex辅助离线补丁，不支持HOME传输

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-01
阶段：进行中

2026年11月1日23:09:04（北京时间），Trey Gwn（@treygwinn）在讨论Wokann的Pokémon Bank离线补丁时称Codex缩短制作时间：据其观察从八月做起、三个月发布，并声称Bank四个月后关闭。这些是评论者的工时推断和停服说法，不是本合集核实的官方时间表或AI效率对照。补读父串中Professor Rex于10月31日22:00的发布转述，称可下载现有线上宝可梦备份、保留3DS存取及离线Poké Transporter，并恢复旧神秘礼物；父帖早于本候选窗口，只作背景。

进一步阅读Wokann/bank_and_mover_offline_patch固定提交c709ec4d28cda0d7935b9ac11bc256e5b841e468的README；提交时间11月1日19:05:24北京时间，早于窗口。项目明确披露使用包括OpenAI Codex在内的AI工具辅助分析反编译输出、设计补丁、写代码和审阅。目标是让Nintendo 3DS上的Pokemon Bank及Poke Mover（Transporter）继续本地工作；离线模式由本地假服务器回答原本的服务请求，文档特别说明这是社区自定义架构，不代表官方服务器设计。

项目文档描述本地存取、箱子管理、多用户和按配置重现礼物；Mover把受支持的第五世代与VC第一／二世代存档转入本地Bank。可在官方服务仍可用时下载线上Bank，但本地数据不能直接上传回服务端；不支持Pokémon HOME传输，不能伪造官方认可的tracker ID。服务器筛查仅模拟社区已知规则，并非完整复刻。部分旧版VC转换与中文编码选项默认关闭，范围受限；不概括成所有世代数据完全兼容。

README要求备份Bank和游戏存档，使用受支持的v1.5基础应用与Luma3DS；构建所需原始解密／解压代码、ExHeader与RomFS须由用户合法取得，不随仓库分发。文档还警告强制解锁不匹配存档可能丢失上次未完成传输的宝可梦。公开文档和AI披露提供可检查的实现背景，不是存档无损、官方规则等价或安全审计证明；未下载原作、构建补丁、运行3DS或独立复测。REA未提及。

候选快照0赞、30浏览、0转发；不借用父帖热度作为本候选快照。
三个月与停服四个月为评论者说法；AI参与有项目明确披露，功能仍未在本合集运行。

## 来源

- [候选：Trey Gwn的Codex与工时转述，2026-11-01](https://x.com/i/status/2116910402646769836)
- [补充父串：Professor Rex的发布介绍，2026-10-31，早于窗口](https://x.com/i/status/2116530772488184281)
- [补充：固定项目README及AI披露，2026-11-01 19:05提交，早于窗口](https://github.com/Wokann/bank_and_mover_offline_patch/blob/c709ec4d28cda0d7935b9ac11bc256e5b841e468/README.md)

[English](en/wokann-pokemon-bank-mover-codex-offline-patch.md) | [返回目录](../README.zh-CN.md)
