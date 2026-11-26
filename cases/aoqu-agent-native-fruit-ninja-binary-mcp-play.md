# Fruit Ninja二进制到MCP：Kimi K3把实时挥砍移入auto_play的三局对照

分类：游戏与游戏保存 · REA
记录日期：2026-11-26
阶段：分析测试

2026年11月26日03:01:26（北京时间），Ao Qu（@ao_qu18465）以Fruit Ninja介绍Agent-Native Computer Use：Agent从既有软件的编译二进制研究内部状态，构建适合自身调用的MCP服务，不必逐屏操作。11:31:04的新候选转述同一研究的FreeCAD和Fruit Ninja结果；两者是独立目标，不把CAD的55倍速度／35倍Token用于游戏。本轮补读此前FreeCAD记录已引用的固定研究正文c822a0c，补足游戏方法与结果；这是既有公开研究的补充阅读，不是本轮新增试验。

文档称Kimi K3只拿游戏二进制和REA、无源码／文档／网络，按研究、运行验证、建服务和检查调用的流程制作MCP，再与看屏computer use各玩三局60秒。带REA服务总分为287、328、299，均值304.7；看屏为74、66、63，均值67.7；不带REA建的服务为115、198、109，均值140.7。总分含终局奖励，不能直接等同实际挥砍水平：对局得分分别为202／243／229、9／6／3、40／137／93，项目概括均值225、6、90。

服务中的auto_play每秒多次读取游戏进程内水果和炸弹的位置／速度并自行挥砍，模型一局通常只调用一至三次，不能写成LLM逐帧或逐刀实时推理。不带REA的服务改为每秒30帧截图、至少三帧追踪，并模拟每次200ms鼠标挥动；文档把收益区分为实时决策移到服务，以及从窗口观察改成内存状态。附录列get_state、auto_play、slash、start_mode和restart_round五工具。

这些是项目正文、图表替代文本和方法的报告，已读但未复跑；未审服务源码、完整原始日志、视频或游戏版本／平台，也没有人类对照或泛化评测，expert-level仍是作者定性。未来随任务继续改工具是展望，不是已实现持续适应。未运行游戏、下载资产或安装依赖，保留analysis-test；REA参与由固定正文明确，不再标未确认。

原介绍与FreeCAD共用快照：22赞、1227浏览、5转发、6回复，不计两次独立验证。
11:31转述候选封存0赞、171浏览、0转发、2回复；本轮已读固定方法文档，未运行测试。

## 来源

- [Ao Qu的Agent-Native Computer Use与Fruit Ninja实时玩法宣称，2026-11-26 03:01:26北京时间](https://x.com/i/status/2125666188630073806)
- [FreeCAD与Fruit Ninja研究结果转述，2026-11-26 11:31:04北京时间](https://x.com/i/status/2125794440963035505)
- [补读固定研究正文：Fruit Ninja三局分数、消融与auto_play机制，2026-11-26作者研究，本轮未产生新实验](https://github.com/MIT-MI/Agent-Native-Computer-Use/blob/c822a0c47cdea82fa28b3955a4216c80f1cc5db9/index.html)

[English](en/aoqu-agent-native-fruit-ninja-binary-mcp-play.md) | [返回目录](../README.zh-CN.md)
