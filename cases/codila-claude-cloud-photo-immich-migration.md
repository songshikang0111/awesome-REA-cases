# 云照片迁至Immich：codila介绍Claude辅助复用iCloud与Google Photos私有请求

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-31
阶段：待验证

2026年10月31日05:22:34（北京时间），codila（@0xCodila）介绍Claude Code／Opus 5.5辅助的一体化照片迁移流程：先检查Mac或Windows电脑空间、磁盘与照片位置，再部署Docker、开源相册Immich和Tailscale私有连接，准备外置盘备份。目标是将云端照片放到自有电脑，并让手机继续备份、远程浏览，减少存储订阅依赖。

作者把iCloud下载原始文件和Google Photos网页内重复私有请求导出称为逆向部分：前者称Apple密码只在本机终端输入，也提供Mac Photos／iCloud for Windows先下载的替代路径；后者称无需等待Takeout。作者还称会对照云端清单核对N/N文件，不删除云端原件，扫描两个二维码后开启手机备份。这些是流程主张，没有给具体库大小、实际导出数、元数据／相册／Live Photo完整性结果或错误处理日志；文件数相同不能独自证明内容、版本和元数据无损。

补查确认作者和正文；未取得所称完整提示及仓库，也没有审计网页脚本、认证处理或网络请求。复用Immich与Tailscale不等于Claude重新实现两个云相册，私有接口可能变化；“完全私密”“永不满”“免费”及可取消订阅均未证明，电脑容量、在线可达性、备份和运行成本仍需考虑。没有输入密码、访问账户、执行脚本或迁移照片，REA未提及。

候选快照42赞、1333浏览、2转发；N/N是流程描述，不是已取得的导出计数。

## 来源

- [codila的Claude云照片迁移指南，2026-10-31 05:22:34](https://x.com/i/status/2116279618894516660)

[English](en/codila-claude-cloud-photo-immich-migration.md) | [返回目录](../README.zh-CN.md)
