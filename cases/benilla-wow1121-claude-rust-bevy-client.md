# benilla：Rust／Bevy重建WoW1.12.1客户端，Claude归因来自转述

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-02
阶段：进行中

2026年11月2日20:32（北京时间），grokked（@grokkedd）介绍benilla，称以Claude、Rust与Bevy重写2006年World of Warcraft 1.12.1客户端，使用自备数据和兼容服务器保留任务、专业、团本、战场、社交、交易、邮件与拍卖行。AI分工是转述归因，未从开发者记录独立确认。

补查samwhosung/benilla的README及差异文档节选，固定提交6a5f0f1064ef52788a92b8b81dffb39958ced71b为11月2日18:41:22北京时间。项目称自行实现格式、原协议和FrameXML／Lua引擎，不含原客户端代码、第三方WoW crates或游戏资产，同时注明早期参考wowemulation-dev与warcraft-rs。完整游玩是项目声明；设置与ESC菜单有意采用Classic Era风格，另有逐项差异，不是逐字节完全等价。

README要求合法取得1.12.1 build 5875数据，开发使用英语客户端与vmangos。服务器不得强制Warden或要求MPQ以外的客户端修改；Warden及其他资料片不在计划。插件兼容、剩余选项、性能和细小差异仍推进，无预编译下载；称可在macOS、Linux、Windows构建。MIT／Apache-2.0覆盖项目代码，不授权Blizzard内容。

另读benilla-re固定README，提交fc85dad3cb85dec9330fb259a87f9d01eea5c68e为10月31日23:10:11北京时间，早于窗口。它按WoW.exe地址记录函数、结构和置信度，描述模拟器执行原函数与Rust逐位差分；生成表与测试要自备匹配版本，其他版本匹配只是线索，不是语义证明。这些是补充项目方法，不是本轮新实验或本合集重跑。候选所称500星、99分支、558提交未核为当前统计；未下载资产、编译或连接服务器。

候选快照19赞、376浏览、1转发；Claude归因是转述，功能与差分验证是项目报告，未独立复现。
不分发游戏数据；不支持Warden，不等于官方服务可用或Blizzard认可。

## 来源

- [grokked转述benilla与Claude重写，2026-11-02](https://x.com/i/status/2117233457667403885)
- [补充benilla固定README：功能与运行边界，2026-11-02](https://github.com/samwhosung/benilla/blob/6a5f0f1064ef52788a92b8b81dffb39958ced71b/README.md)
- [补充固定差异文档节选，2026-11-02](https://github.com/samwhosung/benilla/blob/6a5f0f1064ef52788a92b8b81dffb39958ced71b/docs/DEVIATIONS.md)
- [补充benilla-re固定README：地址与差分方法，2026-10-31，早于窗口](https://github.com/samwhosung/benilla-re/blob/fc85dad3cb85dec9330fb259a87f9d01eea5c68e/README.md)

[English](en/benilla-wow1121-claude-rust-bevy-client.md) | [返回目录](../README.zh-CN.md)
