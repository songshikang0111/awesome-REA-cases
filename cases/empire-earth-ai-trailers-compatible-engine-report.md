# Empire Earth征服的艺术：Claude署名重建、原版混合联机与未覆盖范围

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-12
阶段：进行中

2026年11月12日16:30:18（北京时间），yibie（@yibie）介绍Protryon/empire_earth，称重建引擎可与原版混合host／client联机，AI证据在提交trailer而不在README。补读073017a6b1809735d2d586f633ce7b8ddc2b4584的README，提交于11月8日15:31:23北京时间，早于候选。目标实际为Stainless Steel Studios／Sierra2002年的Empire Earth: The Art of Conquest，重建可由原VC6工具链编译的C++，覆盖游戏和第一方DLL。

固定文档自报11月7日源修订698ba84314bf的游戏代码15420／16884函数（91.3%）和1820263／2736250代码字节（66.5%）匹配；WON库、引擎、网络、渲染等另计。未匹配函数仍以重建源码链接，整文件不是零差异；DCL压缩库明确为格式兼容重实现而非原库机器码。所有映像可从源码链接，不等于所有函数都已匹配。

项目报告短局、长Deathmatch、脚本人类玩家、跨方向存取档及模拟／AI／渲染状态逐tick对照；混合原版和重建host／client的TCP游戏到结束无失步。另有大厅和Direct Connect启动测试，但该界面测试未展示局内peer sync，不能将其和更强的自动联机测试混淆。WON在线服务器已不存在而未测，音频输出与物理输入尚未覆盖。主分支有意保留原版bug以兼容，fixes-all会改变模拟／AI，只适合与同分支联机，不能把混合互通泛化到所有分支。

补查固定修订可达的GitHub提交列表返回22项，均带Claude Opus5.5共同署名；这与候选20处的计数不同，分别保留口径，不把22当AI贡献函数数或完整开发审计。只阅读提交信息和README，未核AI会话、所有测试日志或实现；公开可读也不等于有通用开源授权，README明确No license is granted，需自备合法游戏数据。本合集未构建、联网对战或执行代码，保持进行中。

候选整帖封存3赞、275浏览、0转发、1回复；候选称20处trailer，固定历史读取22项，计数对象不是功能正确率。

## 来源

- [yibie的Empire Earth混合联机与AI提交署名介绍，2026-11-12 16:30:18北京时间](https://x.com/i/status/2120796315898777815)
- [补充固定Empire Earth README，2026-11-08 15:31:23北京时间提交，内含11月7日测量](https://github.com/Protryon/empire_earth/blob/073017a6b1809735d2d586f633ce7b8ddc2b4584/README.md)
- [补充固定历史入口：读取可达提交的Claude Opus5.5署名，非运行验证](https://github.com/Protryon/empire_earth/commits/073017a6b1809735d2d586f633ce7b8ddc2b4584)

[English](en/empire-earth-ai-trailers-compatible-engine-report.md) | [返回目录](../README.zh-CN.md)
