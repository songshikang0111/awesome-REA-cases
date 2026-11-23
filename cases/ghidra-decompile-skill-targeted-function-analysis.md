# ghidra-decompile：先导入、再按地址让Agent研究单个函数

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-23
阶段：相关项目

2026年11月23日16:05:06（北京时间），Laurent Cheylus（@lcheylus）介绍ghidra-decompile Agent Skill及22个Ghidra脚本。补查公开仓库ioma8/ghidra-decompile-skill，目标是避免为了读一个函数先做数小时全量自动分析：先以-noanalysis导入并保留项目，再按精确地址反编译。技能还涉及image base地址对齐、结果核对，脚本覆盖交叉引用、vtable／RTTI和PACIASP入口扫描。介绍者不等于项目作者。

补读固定提交0a7ed092d2ce78d710d4f91a960c2d6a78ccf8d3的README，提交时间2026-11-18T22:44:27Z，早于候选窗口，只作项目补充资料。文档报告114MB去符号AArch64镜像导入后单个目标函数3.3秒；未给硬件和完整测试日志，不能当全镜像恢复或通用加速比。文档称验证于Ghidra12.2，提醒GhidraMCP7.0.0发行包面向12.1.4、与12.2有兼容问题；headless路径不需要MCP。所读仅介绍与README，未安装脚本、分析镜像或复测，也未确认使用REA。

封存快照1赞、38浏览、1转发、0回复；3.3秒为项目文档自报的单函数结果。

## 来源

- [Laurent Cheylus介绍技能，2026-11-23 16:05北京时间](https://x.com/i/status/2124776238636003682)
- [补充README，固定2026-11-18T22:44:27Z提交](https://github.com/ioma8/ghidra-decompile-skill/blob/0a7ed092d2ce78d710d4f91a960c2d6a78ccf8d3/README.md)

[English](en/ghidra-decompile-skill-targeted-function-analysis.md) | [返回目录](../README.zh-CN.md)
