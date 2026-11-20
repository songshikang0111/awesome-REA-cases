# CPS-2 Recomp：Claude署名参与街机原生重编译，时序对照仍有缺口

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-20
阶段：进行中

2026年11月20日16:30:12（北京时间），yibie介绍tmcleroy/cps2recomp：把卡普空CPS-2街机游戏程序译成C++，在项目自写的机器环境运行，支持macOS、Linux、Windows和Android，格斗游戏加入训练与回滚联机。补读固定提交fcd63e519796b8a3948e3c946b1d5bb85c23ae1b的README和ARCADE_ACCURACY，项目还包含部分CPS-1游戏。它称不是模拟器，但仍重建视频、声卡和板级行为，不能由这个标签推出完全没有硬件行为建模。用户需自备指定版本ROM与必要key，仓库不提供游戏数据。

补充提交ec0fdfff30132f02f7fd1bc0be6becd151fad140在11月20日15:14:56北京时间署名Claude Opus5.5，说明时序精度文档工作；前一修改f333656也署名Claude，针对玩家报告Hyper Fighting与Super Turbo过快，默认启用板级等待与DMA时序。两者早于严格16:00窗口，只作AI分工与方法补证，不是本轮新帖子。

项目文档以Verilator模拟的jtcps2／jtcps1为参考，不是实物板。SFA2旧设置报告5671帧中5639帧工作RAM匹配；计入DMA调度后为5634／5671，启动有固定11帧偏移，DMA每帧差约0.16%。Hyper Fighting按测试用10MHz参考比较，战斗速度差约0.2%，实际游戏用12MHz。数值是项目报告，不是本合集复跑。

文档明确Vampire Savior约2000帧后永久分歧、部分RAM区域排除、声画与帧内行为未完整比较、QSound参考被stub、附加模式时序不精确，以及harness与输入脚本仍只在作者机器上。README的Arcade perfect选项不等于已证明街机完美。本合集未构建、下载ROM、运行目标或独立核验联机；保留in-progress，不把所有游戏可玩或模型比较推广为实机等价。

候选封存0赞、153浏览、0转发、0回复；201星为列表快照，热度不验证街机精度。

## 来源

- [yibie介绍CPS-2 Recomp，2026-11-20 16:30:12北京时间](https://x.com/i/status/2123695393049604396)
- [补充：11月20日15:47:20北京时间固定提交的README](https://github.com/tmcleroy/cps2recomp/blob/fcd63e519796b8a3948e3c946b1d5bb85c23ae1b/README.md)
- [同版本ARCADE_ACCURACY：比较方法、差异与未公开harness](https://github.com/tmcleroy/cps2recomp/blob/fcd63e519796b8a3948e3c946b1d5bb85c23ae1b/docs/ARCADE_ACCURACY.md)
- [补充：Claude署名时序精度文档提交，11月20日15:14:56北京时间](https://github.com/tmcleroy/cps2recomp/commit/ec0fdfff30132f02f7fd1bc0be6becd151fad140)
- [补充：Claude署名默认板级时序修复，11月20日13:43:17北京时间](https://github.com/tmcleroy/cps2recomp/commit/f333656cf99d1794d2e072e357b31cd01adc06ce)

[English](en/cps2recomp-claude-native-arcade-recompilation.md) | [返回目录](../README.zh-CN.md)
