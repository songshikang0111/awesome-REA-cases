# Kindle微信读书：丁洪Liam把既有越狱、KOReader与SimpleUI串成Agent安装Skill

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-20
阶段：相关项目

2026年10月26日09:28（北京时间），丁洪Liam（@ding_liam）介绍v0.1安装Skill，希望让自己的Kindle用现代主页阅读微信读书，减少越狱、安装及配置的手工操作。作者称把Skill交给Claude Code、Codex、Cursor或Grok Bot，经USB连接与屏幕确认完成安装；默认启用乔木SimpleUI，提高微信扫码登录卡片优先级，并调整社区插件交互。作者报告自己的Kindle Paperwhite第7代、固件5.16.2.1.1实测跑通。

本轮公开仓库搜索找到LiamZJU/kindle-weread-skill，README中的v0.1介绍、型号、固件和用途与候选对应。补充静态阅读对应93b1ef8caa048cb81c09fd20fa8c1798e33ee392，提交时间为10月26日04:12:51北京时间，早于候选；不是新的窗口帖子。文档明确复用WinterBreak/AdBreak等社区越狱、KOReader、finlater的weread.koplugin和乔木SimpleUI，而非新漏洞发现、重写Kindle固件或运行官方Android微信读书App。脚本负责识别磁盘、下载钉住版本并校验哈希、写入安装包，需要屏幕操作时暂停；这比“完全不用自己动手”的宣传更有限。

README将成功定义为首次进入SimpleUI、用户在手机获取自己的微信读书API Key并扫码登录、打开书籍显示正文；只报告一台KP3、G090前缀、5.16.2.1.1已验证，其他型号和固件未验证。文档警告保修、变砖和第三方客户端账号风险，并提供恢复路径，但电脑无法识别磁盘时工具不能修复；这些不是本合集核验过的安全或恢复保证。未请求、读取或使用任何账号凭据，未安装Skill、下载安装包、连接Kindle、执行目标脚本或独立复现。REA未在候选中声明，按AI辅助旧设备改装的相关项目收录，与基线Android固件移植及Tailscale/Readeck方案不同。

2026年11月20日22:28:40，Nana（@3333yyds）说把价值约200元的旧电子屏通过Codex或Claude Code装上KOReader、微信读书插件与SimpleUI，再WiFi推书和在设备上与AI聊天、看流式输出，必要时让Agent改主题。所给Skill短链确认指向LiamZJU/kindle-weread-skill/tree/v0.1，故补同一工具而非另造固件项目。其流程还提双语EPUB桌面工具与Obsidian投递，未逐个核实，不将配套能力归为Skill自带。没有具体型号、固件、日志或对照；原公开KP3单机验证不能因此变跨型号认证。作者提醒备份、保修、变砖、插件账号与系统分区风险；不收集API Key、不连接设备、不重复操作，保留体验自述边界。

候选热度快照（2026-10-26）：35赞、2400浏览、8转发；不以补查时增长后的数字替换。
仅项目报告KP3/5.16.2.1.1验证，其他型号未验证；复用社区越狱，不是新漏洞或Android移植，未独立运行。
Nana候选封存52赞、1167浏览、0转发、25回复；约200元是旧设备自述，不是改装总成本。

## 来源

- [候选：丁洪Liam介绍Kindle微信读书Skill及单机实测，2026-10-26 09:28北京时间](https://x.com/i/status/2114529444446818627)
- [补充公开README：93b1ef8固定提交，2026-10-26 04:12:51北京时间](https://github.com/LiamZJU/kindle-weread-skill/blob/93b1ef8caa048cb81c09fd20fa8c1798e33ee392/README.md)
- [Nana的旧屏阅读与AI聊天体验，2026-11-20 22:28:40北京时间](https://x.com/i/status/2123785602684617176)

[English](en/ding-liam-kindle-weread-agent-installation-skill.md) | [返回目录](../README.zh-CN.md)
