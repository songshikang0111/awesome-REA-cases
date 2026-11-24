# REA接Trail of Bits技能：Archive建议先读发布二进制再做七类审计

分类：应用与客户端 · REA
记录日期：2026-11-25
阶段：待验证

2026年11月25日01:37:34（北京时间），Archive（@ArchiveExplorer）建议在Claude Code把REA放在Trail of Bits技能前面，针对自己发布的二进制与闭源SDK，先打开目标再检查。帖子列七种职责：dwarf-expert读DWARF调试信息，zeroize-audit查秘密清零，firebase-apk-scanner查Firebase配置，burpsuite-project-parser读已有Burp记录，constant-time-analysis查时序问题，audit-context-building理函数假设，yara-authoring产检测规则。它是具体的授权构建审计idea，不是已发现七类漏洞。

本次补读trailofbits/skills公开main README，确认上述插件名称、Claude Code市场入口与对应用途；这是窗口后可变文档读取，不冒充候选时固定版本。README将zeroize限定在C／C++与Rust，DWARF需要目标保留相关信息，Burp解析需要已有抓取；不能概括成任意剥符号App无需源码即可全自动审计。文档未验证REA组合，也未核99个skills总数、五分钟配置或所有操作零费用。未安装技能、运行构建或检查实际发现，模型/API成本另计；不把安全团队替代宣传当实验结论。

候选封存19赞、1346浏览、5转发、0回复；99技能、零费用与五分钟为宣传口径，未核数量或耗时。

## 来源

- [Archive的REA加Trail of Bits发布构建审计idea，2026-11-25 01:37:34北京时间](https://x.com/i/status/2125282694372180094)
- [补充：Trail of Bits Skills公开main README，本轮窗口后读取，非固定版本或组合验证](https://github.com/trailofbits/skills/blob/main/README.md)

[English](en/rea-trailofbits-release-binary-audit-workflow-idea.md) | [返回目录](../README.zh-CN.md)
