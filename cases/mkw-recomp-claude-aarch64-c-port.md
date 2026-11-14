# Mario Kart World原生PC：Claude写多数代码，AArch64转C但不等于原始源码

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-14
阶段：进行中

2026年11月14日16:30:11（北京时间），yibie的三项目候选提到Mario Kart World，称Claude完成大部分移植，AArch64提前转C，没有解释器或JIT。公开列表给出adriadam10/mkw-recomp；补读固定c06721d README，其提交日期2026-11-14 08:57:37 UTC，晚于候选但仍在本窗口，仅作补充证据，不另建候选。

目标是把Nintendo Switch 2的Mario Kart World 1.0.0／1.8.0以静态重编译带到Linux和Windows。README说游戏CPU代码提前转C，Linux另支持AArch64，NVN2在Vulkan上重实现，SM86着色器预先转SPIR-V，部分Nintendo SDK函数按符号替换。这是机器码转译与宿主兼容，不是找回原开发者的C源码。继承TotK Recomp及社区平台／着色器研究，不能说Claude独自从零发现整个平台。

作者称Claude做大部分输入，人类指导，约十天全职、从10月30日起489次提交，每次先审阅、测量或测试；并明确不是一条提示完成。性能改动在同次运行内A/B，因为不同运行可相差12ms；画面修复对照原机图，着色器改动在11561个程序上离线测后才跑游戏，抓帧回放帮助定位。数字与流程均为项目说明，本合集未核计提交、读取所有测试或确认每条门禁实际执行。

文内11月12日状态报告Linux／Windows x86-64可启动、进菜单与比赛，Linux AArch64在Adreno740掌机测过；仍有菜单、阴影、电影音频与部分AMD挂起问题，没有在线联机。11月9至11日表格列高端卡60fps、GTX1650 SUPER约24fps等，不能把局部60fps当所有设备流畅，补帧也不等于游戏逻辑更快。用户需自备游戏，项目MIT与第三方条款不授权游戏资产。本合集未下载目标、构建或跑比赛，REA未提及，保留进行中。

共享候选封存2赞、259浏览、0转发、1回复；720星为当日转述，约十天、489提交与11561着色器均为项目统计。

## 来源

- [yibie本窗口三项目介绍：Mario Kart World，2026-11-14 16:30:11北京时间](https://x.com/i/status/2121521061955244445)
- [补充mkw-recomp固定README：Claude方法、性能与已知问题，提交2026-11-14 08:57:37 UTC](https://github.com/adriadam10/mkw-recomp/blob/c06721d1a8fcc8fab3b4532ec4ea6badc73c485e/README.md)

[English](en/mkw-recomp-claude-aarch64-c-port.md) | [返回目录](../README.zh-CN.md)
