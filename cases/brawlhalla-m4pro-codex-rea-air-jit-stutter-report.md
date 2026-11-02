# Brawlhalla卡顿：Codex／REA追到AIR在Rosetta下的解释器分支

分类：游戏与游戏保存 · REA
记录日期：2026-11-02
阶段：分析测试

2026年11月2日15:48:28（北京时间），fexx_off（@fexx_off）报告MacBook Pro M4 Pro运行格斗游戏Brawlhalla时短暂冻结，离线Training也发生，超过两名玩家的Free-for-all更明显。作者使用Codex、GPT 6.1 sol与REA调查；调整FPS目标、全屏和干净启动后仍有卡顿，全屏只部分改善。

作者称REA帮助检查已安装应用并收集证据，原生堆栈采样与二进制检查将问题指向随游戏附带的Adobe AIR运行时：该构建检测到Rosetta后主动选择ActionScript解释器，而非JIT即时编译。研究找到既有配置覆盖AS3JIT=2，先备份共享配置、临时测试并在启动后自动恢复；新采样不再显示此前反复出现的解释器调用路径。随后作者亲自玩Training与Free-for-all，均称冻结“基本消失”，再让Sol为普通Steam启动持久化设置。

这是作者报告的症状、运行时决策、配置试验、重新采样与人工试玩链，不是本合集复现。未公开游戏／AIR版本、定位地址、堆栈、完整配置位置、帧时间分布、测试时长或回退后的对照，不能保证所有Mac、AIR版本或模式均有效，也不能由一个调用路径消失量化性能收益。补取原帖确认作者与全文，未运行游戏、修改配置或取得独立测试。

封存候选快照1赞、21浏览、0转发；不是热度优胜或独立验证。
AS3JIT=2与两种模式的改善为作者报告，无量化帧时间或原始采样。

## 来源

- [fexx_off的Codex／REA采样、AIR分支与试玩报告，2026-11-02](https://x.com/i/status/2117161909883408416)

[English](en/brawlhalla-m4pro-codex-rea-air-jit-stutter-report.md) | [返回目录](../README.zh-CN.md)
