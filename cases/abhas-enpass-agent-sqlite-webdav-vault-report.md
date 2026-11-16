# Enpass给Agent单独的保险库：Abhas称研究加密SQLite后经WebDAV与App共用

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-16
阶段：待验证

2026年11月16日10:49:05（北京时间），Abhas Bhattacharya（@abhas_tweeter）说许多应用不适合Agent操作，自己因此研究过包括离线优先密码管理器Enpass在内的应用。他也承认密码管理器并非理想的computer-use目标，改从数据库层接入。

作者称Agent逆向了加密SQLite数据库，包括TOTP、passkeys与附件；随后给Agent一个经WebDAV同步的独立vault，并将同一保险库加入Enpass App。其报告用途是让Agent为新VPS、部署自托管应用等任务添加密码／密钥，并读取他主动复制进该vault的条目。这里是研究文件结构与应用互通的自述，不是证明在没有密码或授权的情况下解密保险库，也不是把全部个人保险库开放给Agent的报告。

帖子未说明模型、REA、Enpass版本、数据库结构、解密流程、写入校验、冲突处理或权限机制，没有代码、测试记录与安全审计。单独vault是作者的操作安排，不保证进程隔离、凭据不会泄漏或WebDAV端到端安全。补取只确认署名与全文；本合集未接触任何保险库、密码、密钥或私有服务，不复述敏感条目。保持unverified，不推荐据此直接接入生产凭据。

2026-11-16封存候选：0赞、5浏览、0转发、0回复；未给开发工时或安全评估。

## 来源

- [Abhas的Enpass数据库与独立WebDAV保险库报告，2026-11-16 10:49:05北京时间](https://x.com/i/status/2122159995806708136)

[English](en/abhas-enpass-agent-sqlite-webdav-vault-report.md) | [返回目录](../README.zh-CN.md)
