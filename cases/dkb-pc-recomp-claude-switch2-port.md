# Donkey Kong Bananza PC：Claude辅助静态重编译，仍有GPU崩溃与后段缺陷

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-14
阶段：进行中

2026年11月14日16:30:11（北京时间），yibie的列表更新同时介绍三个独立项目，本条只记录Donkey Kong Bananza PC。候选称FAQ明确多数代码由编码Agent写、以运行游戏及差分测试检查。补读其公开列表取得Lucas-blip-png/dkb-pc-recomp，再读固定fac48bc README，提交日期2026-11-13 14:20:24 UTC，文内状态更新日11月13日；它是较早补充材料，不是新候选。

项目目标是把Nintendo Switch 2的Donkey Kong Bananza带到原生Windows x86-64。文档称ARM64代码预先转C再编译，运行时不用CPU模拟器，NVN2图形接口由Vulkan宿主承接；基础来自TotK Recomp，着色器还使用Eglantine的Ampere降级及Ryujinx相关翻译器。AI归因是Claude Code编写大多数代码和文档，人类负责阅读与运行，不是从零独立发现全部平台知识。

状态表报告180061个函数无不支持指令并通过Unicorn差分测试，首个3D场景4820个着色器阶段经翻译；这些是项目检查结果，不等于完整游戏行为或视觉无差异。文档称近期NVIDIA卡可玩至第一关之后，但列NVIDIA／AMD device lost、RADV挂起、后续区域guest崩溃、缺特效及重场景低于60fps。新默认设置在项目重场景约53到58fps，仍有约0.45秒区域加载停顿；不是本合集基准。旧FAQ仅描述RTX5060Ti手玩首关，不能忽略同文较新的玩家报告，也不能把后者当全程通关。

自备1.0.0或3.2.0数据；3.2.0仅报告启动阶段150秒60fps、尚无游玩验证。Linux／macOS是预览，Apple Silicon只核到模式选择且缺破坏地形。项目不附游戏资产，GPL与继承MIT条款不授权Nintendo内容。本合集只读文档，未下载游戏、执行构建、差分或GPU测试；REA未提及，保留进行中。

共享候选封存2赞、259浏览、0转发、1回复；957星为yibie当日转述，不是性能或独立测试。

## 来源

- [yibie本窗口三项目介绍：Bananza，2026-11-14 16:30:11北京时间](https://x.com/i/status/2121521061955244445)
- [窗口前DKB固定README：AI归因、状态与限制，提交2026-11-13 14:20:24 UTC](https://github.com/Lucas-blip-png/dkb-pc-recomp/blob/fac48bcdc5ec0edd6296bc3672bdebb540d5958d/README.md)

[English](en/dkb-pc-recomp-claude-switch2-port.md) | [返回目录](../README.zh-CN.md)
