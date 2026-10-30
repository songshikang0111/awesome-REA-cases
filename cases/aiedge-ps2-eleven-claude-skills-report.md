# The Console skill：11个Claude技能组织PS2重编译与mod工作

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-30
阶段：进行中

2026年10月30日13:00:03（北京时间），AI Edge（@aiedge_）转述11个Claude Code技能，覆盖PS2游戏逆向、图形、声音、控制器与代码mod。补充公开检索找到描述高度对应的Jakeschincariol/console-skill，读固定提交a508929f1e8f5dd6f54afe489fd74340df3b6f74的README；提交为10月22日22:14:44北京时间，早于窗口，含Claude Opus5.5协作署名。候选短链未解析，仓库为对应描述的补证，不冒充已经证实短链目的地。

文档把它定位为基于ran-j/PS2Recomp及hkmodd原始skill的原生移植工作流，不是模拟器：MIPS机器码经重编译为C++，再由Agent补运行时、分析Ghidra函数和崩溃日志。共享STATE.md与design.md保存阶段和行为规格；11角色还包括关卡、物理、存档、多平台打包及测试。宽屏、任意手柄、mod与云同步是功能宣称，未逐项验收。

项目称559个离线测试使用合成ELF、光盘、纹理、音频、存档与日志，不包含真实游戏数据；不是559款游戏通过。README明确许多游戏还不能启动、图形和向量单元慢、仍有大量stub，移植可耗数周甚至失败。用户需合法自备游戏，生成C++与资产不应随补丁发布；工具包MIT与PS2Recomp GPL-3.0不能混同为所有目标的授权。本合集未下载游戏、安装技能、编译或重跑测试，不承诺一键可玩或全平台兼容。

候选快照3赞、1842浏览、1转发；未独立运行559个项目合成测试。
固定提交2026-10-22T14:14:44Z；候选短链目的地未确认。

## 来源

- [AI Edge介绍11个PS2 Claude技能，2026-10-30](https://x.com/i/status/2116032360559108398)
- [补充：描述对应的console-skill固定README，10月22日提交](https://github.com/Jakeschincariol/console-skill/blob/a508929f1e8f5dd6f54afe489fd74340df3b6f74/README.md)
- [补充：固定提交与Claude协作署名](https://github.com/Jakeschincariol/console-skill/commit/a508929f1e8f5dd6f54afe489fd74340df3b6f74)

[English](en/aiedge-ps2-eleven-claude-skills-report.md) | [返回目录](../README.zh-CN.md)
