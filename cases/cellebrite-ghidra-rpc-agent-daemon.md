# ghidra-rpc：Cellebrite Labs让Agent用JSON CLI持续研究Ghidra项目

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-05
阶段：相关项目

2026年11月5日09:21:37与09:25:15（北京时间）的候选清单介绍Cellebrite Labs的ghidra-rpc，11:04:02的日文转述进一步列出v0.3.0变化。补查公开仓库固定提交fa3866243dcfcbc876baa7b13ae0deac2c443cd8（11月3日01:02:27北京时间）的README，以及11月3日01:10:50发布的v0.3.0说明；这些是早于候选的项目记录，不是本窗口新测试。

项目用PyGhidra把Ghidra常驻在JVM内，CLI返回结构化JSON，使Claude Code、Cursor等能调用反编译、调用图／交叉引用、重命名注释、类型恢复、指令与字节补丁、BSim函数匹配及版本diff；二进制只加载一次，文档称每条修改命令后保存到项目，GUI可查看。用途是二进制审计、漏洞研究和补丁前后比较，工具能力不等于已完成某个目标的正确逆向。

v0.3.0文档说明Windows用带token认证的127.0.0.1 TCP替代Unix socket，支持headless与GUI，修复--detach在Job Object启动器下退出的问题。search-decompiled返回实际扫描范围和下一未扫地址，支持有界续查；xrefs-to追踪导入thunk链。输出地址统一加0x、裸十六进制改按名字查找、disassemble默认不再返回instructions，均有兼容性影响。发布说明还报告修复中止写事务可能导致下一成功写入在保存时丢失的问题，并使--or-replace失败时保留旧类型。

项目称CI覆盖三系统单元测试及Windows headless集成，GUI无CI覆盖；GUI拒绝version-track与match-function。README列Ghidra11+、Python3.11+、Java17+、uv及MIT许可。这里核对了文档与发布记录，未检查全部实现、运行CI、安装依赖或载入二进制；不能把发布修复说明当成本合集复现、语义正确性或全面平台保证。未确认使用morluto/rea。

三候选封存依次0赞／22浏览／0转发、0赞／43浏览／0转发、1赞／431浏览／3转发；清单称394星，仅为11月5日转述快照。
发布记录的测试覆盖与修复属项目口径；GUI未纳CI，未在本合集运行。

## 来源

- [候选：开源清单提到ghidra-rpc，2026-11-05 09:21:37](https://x.com/i/status/2118151716223017172)
- [候选补证：常驻、JSON与Agent用途，2026-11-05 09:25:15](https://x.com/i/status/2118152633903132784)
- [候选补证：v0.3.0与GUI边界的日文转述，2026-11-05 11:04:02](https://x.com/i/status/2118177490820898823)
- [补充项目README：固定11月3日提交，非本窗口测试](https://github.com/cellebrite-labs/ghidra-rpc/blob/fa3866243dcfcbc876baa7b13ae0deac2c443cd8/README.md)
- [补充项目发布说明：v0.3.0，2026-11-03 01:10:50北京时间](https://github.com/cellebrite-labs/ghidra-rpc/releases/tag/v0.3.0)

[English](en/cellebrite-ghidra-rpc-agent-daemon.md) | [返回目录](../README.zh-CN.md)
