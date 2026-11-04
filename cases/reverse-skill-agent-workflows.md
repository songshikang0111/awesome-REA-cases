# reverse-skill：给编程 Agent 的多目标逆向路线

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-04
阶段：相关项目

较早帖子介绍reverse-skill可放入Codex、Cursor和Claude Code，为APK、前端及固件分析选择工具。10月20日12:19（北京时间）的四条候选进一步说明工作区根目录的AGENTS.md与RULES.md先要求列出命令、写入、网络和全局配置影响并获批准，再由master-route选择唯一PRIMARY，case-init记录授权范围，最后加载专项技能。阅读仓库、安装插件或给样本路径都不等于授权；只复制skills目录会漏掉这些入口规则。这是Agent的调查编排，不是新反编译引擎，也不是自动保证守规。

路由使用must、mustAll、exclude正则规则，按命中数与priority选PRIMARY，无命中回R0。中文越狱与英文jailbreak按移动端或LLM上下文区分。候选称有178条中英文路由基准、Windows和Ubuntu检查；补读zhaoxuya520/reverse-skill公开README、AGENTS、基准JSON与bootstrap源码，确认可检查的实现与178条用例存在，但未运行脚本或CI，不把规模当作178个成功逆向任务。工具索引记录本机路径和版本，bootstrap按清单准备依赖，默认不注册MCP；写Codex或Claude全局配置需显式选择。版本固定与日志脱敏是项目设计，不代表本合集审计了全部依赖或秘密清除效果。

候选给出自有APK的纯离线试用流程，要求先建scope并通过case-guard；没有完整目标分析验收。Windows是完整主路径，Kali有专门脚本，macOS、Ubuntu、Debian为通用支持，IDA保活脚本仅Windows。未安装依赖、改配置或执行目标，不能认定所有平台功能对等或所有格式可靠处理。仓库身份补足此前缺少实现链接的限制；仍作为相关工作流项目，不与apk-reverse混为一谈，未确认使用REA。

2026年11月4日21:29:30（北京时间）的新帖强调先选方法论再调用jadx、Frida或IDA，并将经验沉淀复用，另报44条路由规则、175条回归用例，支持Claude Code、Codex、Cursor。这是新宣传口径，未读取对应固定版本或运行回归；不能覆盖10月已见178条基准，也不能断言三条被删除、测试退步或175个目标成功。

10月20日四条候选快照均0赞，分别86、118、39、139浏览；仅静态阅读公开文件，未运行目标或工作流。
11月4日新帖封存2赞、83浏览、0转发；44规则／175用例为未重跑的新自述，与旧178基准分开。

## 来源

- [本窗口项目介绍](https://x.com/i/status/2110680583634366777)
- [10月20日12:19：规则路由与178条基准](https://x.com/i/status/2112398152686829612)
- [同串：授权、PRIMARY与插件边界](https://x.com/i/status/2112398151613100171)
- [同串：工具索引与显式MCP注册](https://x.com/i/status/2112398154788213150)
- [同串：离线样本与平台支持差异](https://x.com/i/status/2112398155400552729)
- [公开仓库：只读核对文档、基准及bootstrap](https://github.com/zhaoxuya520/reverse-skill)
- [新帖：44规则、175回归用例与经验复用，2026-11-04](https://x.com/i/status/2117972508905459981)

[English](en/reverse-skill-agent-workflows.md) | [返回目录](../README.zh-CN.md)
