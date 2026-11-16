# Horizon：AI辅助以Rust重建Minecraft Java行为，用差分测试对照原版

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-16
阶段：进行中

2026年11月16日14:32:49（北京时间），TechVerser（@realfxw）介绍horizon-rust/horizon：以Rust重建Minecraft: Java Edition 26.3的客户端和游戏行为，摆脱Java运行环境而保留原版玩法、存档和联机。帖子称Claude联合署名提交9900多个、Codex一千多个，并以281套差分测试对齐原版。这些计数未逐项审计；联合署名也不等于AI独立设计、人工零参与或源码原创性的证明。未提REA。

补读公开仓库固定85b5bcca7c79bb470b90bdb5914b413aa66fe7ae的README和提交说明，提交时间为2026年11月16日01:32:47 UTC，即本窗口之前的项目背景，不是新候选。提交说明有OpenAI Codex联合署名，报告合并原生与Wasm mod API、保留分支历史，并称最终头部CI通过；本合集没有另读该CI日志，不能当独立测试通过。仓库公开简介也称281套差分测试，但本次未审测试清单、oracle、样本或逐项结果。

固定README将项目归于Horizon Team，创始人为Ludovic Marie；自述支持生存、创造、极限模式、各维度地形、生物、村民、红石，直接打开存档，连接原版或Horizon服务器、局域网和邀请联机，并有自己的mod系统、光影包及最高1024区块远景。这些是项目功能承诺，非本合集运行确认；候选所说1.8到26.2存档无缝升级未由所读README具体证明，也不把自己的mod API推为兼容全部Java mod。

文档图片文字报告相对装有Sodium、Lithium、FerriteCore和ImmediatelyFast的Java版启动快3.5倍、FPS高38%，限定Ryzen 7 9800X3D与RTX 5080；未读外链基准或重跑，不把候选所说老四核不卡、玩家帧率翻倍泛化成普遍性能。文档要求自有Minecraft Java副本、安装并启动26.3一次；项目称不分发Minecraft文件，而从用户购得游戏生成所需文件。本合集未审提取流程、登录安全或法律主张，候选对DMCA的猜测不是已发生下架。

README称原创工作现用LGPL v3或以后版本，转许可前代码仍有MIT授权，依赖各保留许可；这不授权Mojang/Microsoft代码与资产。补取确认候选署名和文字，未观看图片、安装启动器、登录账号、下载游戏资产或执行目标代码。保留进行中，既不称完全等价，也不称找回原始源码。

候选封存0赞、56浏览、0转发、1回复；约8.2k星为帖子文字快照，非功能验证。

## 来源

- [TechVerser介绍Horizon及AI提交／差分测试，2026-11-16 14:32:49北京时间](https://x.com/i/status/2122216298549588224)
- [窗口前固定README：玩法、存档、性能条件与授权，2026-11-16 01:32:47 UTC提交](https://github.com/horizon-rust/horizon/blob/85b5bcca7c79bb470b90bdb5914b413aa66fe7ae/README.md)
- [同一固定提交：Codex联合署名及mod API合并自述，非独立CI复测](https://github.com/horizon-rust/horizon/commit/85b5bcca7c79bb470b90bdb5914b413aa66fe7ae)

[English](en/horizon-minecraft-java-rust-ai-differential-reimplementation.md) | [返回目录](../README.zh-CN.md)
