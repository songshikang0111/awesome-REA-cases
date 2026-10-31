# Homecloud云照片迁至Immich：Claude串联私有请求与外盘存储

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-31
阶段：待验证

2026年10月31日05:22:34（北京时间），codila（@0xCodila）介绍Claude Code／Opus 5.5辅助的一体化照片迁移：检查Mac或Windows磁盘、部署Docker、开源相册Immich和Tailscale，导入云照片并另做备份，目标是保留手机备份和远程浏览，减少存储订阅。09:22:08同作者再次介绍相同流程。这里是照片自托管迁移，不是重写iCloud或Google Photos服务。

作者称逆向部分是复用云相册网页私有请求下载原件，并对照云端清单核对N/N，最后扫描两个二维码启用手机备份。较早帖子说不删云端原件，较新帖写“nothing in your cloud”，并不构成已删除或已成功迁移的证据。没有实际库大小、完成导出数、相册／Live Photo无损报告或错误日志；N/N是工作流主张而非本合集取得的验收结果。

09:06:00，ElioEx（@elioex0）介绍同类Homecloud路线并明确给出iCloud-reverse-engineered仓库名、外盘参数、新装限制与空间估算。补查定位Bodila51/iCloud-reverse-engineered，静态阅读固定提交c83ea2685e19b6f924d4cdc628ad5f10cc058f9f的README及变更，提交时间为10月31日04:37:39北京时间，早于本窗口。公开文档与codila所述工作流一致，但不从相近名字推定Bodila51就是codila。

项目复用pyicloud做iCloud登录下载、Google Photos Toolkit的请求格式／响应解析做Google网页路线，再导入Immich；并非从零独立恢复全部协议。固定变更把Mac的--upload-location与Windows的-UploadLocation传入安装入口，照片可放常接外盘、数据库留电脑；只对新装生效，已有库不自动迁移。下载后导入通常预留约2.2倍相册空间，100GB示例约220GB，备份另盘；Mac Photos路线还另算Photos库，不适用于所有路径。

README保留重要限制：iCloud会话密钥在退出前可被同用户程序读取，不是绝对私密；Google私有请求可能改变并有条款／账号风险，建议不愿冒险者选Takeout。Google网页清单若不完整，N/N也发现不了；Locked Folder、Trash及别人共享的相册不包括，Storage saver只下载云端保留版本。Mac／Windows的Immich部署有Docker开销且不属Immich推荐环境，手机后台上传受系统限制。项目声明不改删云端文件，降级订阅和关闭同步须用户自行决定，不能由宣传推定可安全取消。

这次取得公开仓库与文档，修正此前仓库未知的边界；没有审计全部认证和下载实现、输入密码、访问账号、执行脚本或迁移照片。费用还包括硬盘、电力和设置时Claude服务；“免费”“永不满”和完整无损未验证，REA未提及。

较早快照42赞、1333浏览、2转发；本窗口ElioEx为1赞／98浏览／0转发，codila为50赞／3935浏览／8转发。
N/N与2.2倍空间为项目流程／估算，非实际导出验收；只静态审读，未运行。

## 来源

- [codila的Claude云照片迁移指南，2026-10-31 05:22:34](https://x.com/i/status/2116279618894516660)
- [ElioEx介绍Homecloud外盘、新装与2.2倍空间路线，2026-10-31 09:06](https://x.com/i/status/2116335848312430784)
- [codila再次介绍私有请求与Immich迁移，2026-10-31 09:22](https://x.com/i/status/2116339908822319428)
- [补充：Homecloud固定README，路线、上游与风险](https://github.com/Bodila51/iCloud-reverse-engineered/blob/c83ea2685e19b6f924d4cdc628ad5f10cc058f9f/README.md)
- [补充：10月31日04:37北京时间外盘安装参数变更，早于候选窗口](https://github.com/Bodila51/iCloud-reverse-engineered/commit/c83ea2685e19b6f924d4cdc628ad5f10cc058f9f)

[English](en/codila-claude-cloud-photo-immich-migration.md) | [返回目录](../README.zh-CN.md)
