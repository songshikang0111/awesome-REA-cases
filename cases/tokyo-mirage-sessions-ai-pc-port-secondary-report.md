# Tokyo Mirage Sessions／TMSRecomp：Claude署名静态重编译，测试到第二章

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-26
阶段：进行中

2026年10月28日06:18:32（北京时间），playswave（@playswave_com）称Tokyo Mirage Sessions已有粉丝PC反编译移植、60至120FPS，放在AI编程叙事中。旧报道未给项目名、作者、仓库、系统、版本、测量或AI工作记录，链接文章未取得，不到100万销量也仅其背景说法；保留历史来源，不认定后来具名项目就是当时同一实现。

11月26日14:50:23，Furkan YILDIRIM（@furkandev）介绍TMSRecomp，将Switch游戏Tokyo Mirage Sessions #FE Encore静态重编译到Windows；转述README称Claude通过Claude Code写所有代码、工具与逆向，人类负责指导、测试、审阅；ARM转C再编为Windows x64，并称可达4K／240FPS、11月23日起三天五个beta。后两项是帖子时间线与性能上限说法，不是工时或本合集测量。按同一游戏目标补到既有ID，不抹平早帖的身份不确定性。

本轮补读godofknife/TMSRecomp固定5807e38667c8a5c4d96c4f69c1d81b063fce7179的README，提交为11月26日04:09:54北京时间，早于本轮窗口。文档确认v0.1.4 beta及上述AI／人工分工，32位ARM静态转C，Vulkan实现所需NVN图形接口，无JIT；列运行时的内存、Horizon服务、音频与输入，以及借Ryujinx译码器将Maxwell着色器转SPIR-V。文档提test_a32.py对照Unicorn，但未读测试实现或结果，不能说翻译已全面通过。

Windows仅报告NVIDIA RTX测试至第二章Idolasphere并存取档，后续章节、AMD／Intel和弱PC未知。需自备Switch基础版1.0.0、无更新，title ID为0100A9400C9C2000；固定地址hook不支持1.0.1+／DLC。4K和30至240或不封顶是可选设置，不是所有场景实测，文档称60FPS测试最多、NPC高帧率转向仍为30Hz步进。另有实验Linux：项目报Ubuntu 26.04／GTX 1650／驱动620，场景和存取档等60FPS，战斗、AMD／Intel与Steam Deck未测，未接FSR3／DLSS；不能把它写成所有平台只测RTX或Linux完整可玩。模拟器存档与更新版存档兼容也未测。

文档称不含游戏，用户本地生成的game.dll包含游戏不可分享；这是分发声明，不是本合集审计整个发布包。未获取游戏、密钥、固件、发布包或依赖，未构建运行、审实现或复现画面／帧率；只核对公开文档与出处，保留项目归因，状态in-progress。REA未提。

旧候选快照0赞、31浏览、0转发；旧60至120FPS及AI归因仅二手文字，不由新项目文档追认。
11月26日候选封存2赞、246浏览、0转发、1回复；三天五个beta为转述，未核发布历史；README仅作为项目自报证据。

## 来源

- [playswave的Tokyo Mirage Sessions移植报道，2026-10-28，未确定与TMSRecomp相同实现](https://x.com/i/status/2115206541045551503)
- [Furkan YILDIRIM介绍TMSRecomp与第二章测试边界，2026-11-26 14:50:23北京时间](https://x.com/i/status/2125844598161346932)
- [补充TMSRecomp固定README，提交2026-11-26 04:09:54北京时间，窗前文档](https://github.com/godofknife/TMSRecomp/blob/5807e38667c8a5c4d96c4f69c1d81b063fce7179/README.md)

[English](en/tokyo-mirage-sessions-ai-pc-port-secondary-report.md) | [返回目录](../README.zh-CN.md)
