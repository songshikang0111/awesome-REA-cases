# DX RUST：Deus Ex的Rust／Bevy重实现，公开文档仍待完整通关测试

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-01
阶段：进行中

2026年11月1日08:15:55（北京时间），候选报道介绍Grissyelda的DX RUST：以Rust与Bevy从头重实现Ion Storm于2000年推出的Deus Ex，读取用户已有GOTY安装中的地图、贴图、声音、对话及类默认值，而不是仅在兼容层运行旧引擎。帖子称0.10.0、73张地图、三个结局及Windows／Linux／Steam Deck支持，AI参与较重，但未量化。

补读固定提交5ca15b0c68141a0b53ef7baac9d91fd96f7c570d的README及提交信息，时间为11月1日01:58:17 UTC，即北京时间09:58:17，晚于候选但仍在窗口内，只作补充一手资料。README自述全游戏已实现，按83个地图文件描述范围，与候选73张的口径不同，不强行换算或确认地图总数。它列原始规则默认、可选现代画面、手柄／DualSense、Mod支持及独立资源读取模块；同时把完整通关、性能优化、Steam Deck调优和每图存档往返测试列为1.0前待做。不能由“已实现”推成全战役验收通过。

该提交author为Claude，提交消息注明Claude Opus 5.5共同署名，GitHub验证标志为true；它涉及阴影、骨骼角色、布料和Mod兼容性修复。这支持AI参与这一提交，不证明模型独自完成整个项目或功能正确。README声明自有代码GPL-3.0-or-later、游戏与Mod文件需另备；其RTX3050现代画面约32到47fps说法也是项目自述。这里只读文档与提交元数据，未构建、运行、计时、核验资产分发或完整通关。

候选快照11赞、660浏览、1转发；补充文档晚于候选，不作为另一候选。
73张地图与83个地图文件为来源不同口径；未独立测试全战役或性能。

## 来源

- [DX RUST与AI参与的候选报道，2026-11-01](https://x.com/i/status/2116685634307760281)
- [补充：11月1日09:58固定README，地图文件口径与待测项](https://github.com/Grissyelda/dx-rust/blob/5ca15b0c68141a0b53ef7baac9d91fd96f7c570d/README.md)
- [补充：同一Claude署名修复提交与验证元数据](https://github.com/Grissyelda/dx-rust/commit/5ca15b0c68141a0b53ef7baac9d91fd96f7c570d)

[English](en/dx-rust-deus-ex-bevy-ai-reimplementation-report.md) | [返回目录](../README.zh-CN.md)
