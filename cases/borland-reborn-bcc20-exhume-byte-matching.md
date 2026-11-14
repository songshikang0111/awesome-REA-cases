# borland-reborn：Exhume辅助重建Borland C++ 2.0，字节一致不是原始源码唯一恢复

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-14
阶段：待验证

2026年11月14日18:32:55（北京时间），@huihoo串中的介绍帖称Abedegno用Exhume恢复1991年Borland C++ 2.0编译器。目标是保存DOS命令行编译器BCC.EXE及独立预处理器CPP.EXE，使可读C与汇编能用原工具链重建，并研究编译器内部机制。候选所称100%恢复全部原始源码需要收窄：字节一致支持某份等价重建，不证明找回开发者原始文本、变量命名或唯一源码。

公开检索找到abedegno/borland-reborn，补读固定提交71530cb的README；其提交时间为2026-11-14 11:10:44 UTC，晚于介绍帖，但仍是另行补充文档，不是新的候选。文档把BCC.EXE与CPP.EXE标为整文件字节相同；BCC部分列298份源码，即265个C文件与33个手写TASM模块，保持原程序中编译C与手写汇编的分工，不把原有汇编强塞成C。约3100个函数／全局／标签、300字段、40布局与约10000行注释是项目可读性整理规模，不是恢复原名的独立证据。

README描述由gate重新编译，逐函数比字节、核重定位与名称，再链接完整BCC.EXE。它另有允许代码增长和移动的modding构建，以1836次编译与原编译器逐输出对照，报告代码覆盖83%；不能把1836当独立用户验收或83%写成全部路径。原生bcc20-port仅刚开始调用记录、回放与首批运行时函数，不与已称匹配的DOS版混成完成移植。

补读Exhume README明确是工具包加Claude Code skills，原提交1602022日期为2026-11-13 23:57:15 UTC，早于本窗口，仅用于核实AI工具关系。Borland项目说明自己的脚本／文档为MIT，恢复源码派生自Borland版权程序，不主张相关权利；复建仍要用户自备原工具。未执行任何安装、目标代码、编译、1836次对照或哈希比对，也未核读FINDINGS全部技术断言。以项目报告而非独立重现收录，REA未提及。

候选封存35赞、2097浏览、6转发、7回复；298源文件、1836次编译与83%覆盖均为项目说明，未复测。

## 来源

- [Borland C++2.0与Exhume介绍，2026-11-14 18:32:55北京时间](https://x.com/i/status/2121551947186704540)
- [补充borland-reborn固定README，提交2026-11-14 11:10:44 UTC](https://github.com/abedegno/borland-reborn/blob/71530cbfe35cb6ed64892f7096b12da710939021/README.md)
- [窗口前Exhume固定README：Claude Code skills，提交2026-11-13 23:57:15 UTC](https://github.com/abedegno/Exhume/blob/160202277647e7e97cca8a06e76184f88c573748/README.md)

[English](en/borland-reborn-bcc20-exhume-byte-matching.md) | [返回目录](../README.zh-CN.md)
