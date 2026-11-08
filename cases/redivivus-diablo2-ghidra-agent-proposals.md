# Redivivus：Agent只读研究暗黑II数据库，以提案修正C++重建

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-08
阶段：进行中

2026年11月8日16:30:20（北京时间）的资源日报介绍jaenster/redivivus：agents为Diablo II: Lord of Destruction 1.14d的Ghidra数据库提出名称与类型修正，MCP只读，写入发生在提案层。目标是把发行版Game.exe恢复成可构建C++，用于单人游戏研究和保存，而不是另写一个相似游戏或接入Battle.net。

补读窗口内18:35:56提交bb149dcad7fd53c59f6d0d1d305a0f8656263a5f的README、CONTRIBUTING和BYTE-MATCHING：源码树大多从Ghidra数据库生成，因此名称、类型、原型和调用约定问题应按原地址提交证据，经检查与审阅后应用，而不是直接改会被覆盖的生成文件。指南提供Claude Code插件，其他Agent也可读Windows与同源Intel Mac数据库；函数发现／边界变更另走人工issue流程，生成器错误应修ghidra-reconstruct。数据库可读不是任意写权限，也不是无人审查的Agent自动修复。

该固定README自报数据库v2035、22个模块库，严格C++17编译和无未定义符号链接；Visual C++ 2005构建已完成一次单人通关。以原编译器Visual C++ 2005 SP1比较，7772／14626函数匹配（53.1%），整函数匹配代码629221／2598518字节（24.21%）；去掉625个已恢复但无直接引用的匹配函数后是7147／14626（48.9%）。地址字段按所指对象归一比较，并非整EXE逐字节相同；主指标排除C运行库、编译器异常辅助代码和PKWARE库。x64的464个文件可编译仍不等于x64可玩，另有1114处指针宽度转换。

README保留NPC任务滚动文本不出现及偶发崩溃，单人任务仍可推进；不支持Battle.net。需要自有1.14游戏安装，仓库不含游戏数据。文档感谢blizzhackers、D2MOO等既有人工研究，不把全部恢复归功AI。补充文档于11月9日取阅，固定提交虽晚于日报但仍在本窗；构建、通关与匹配都是项目自报，本合集未执行代码、下载游戏或重跑oracle，REA未提及。

候选封存1赞、288浏览、0转发；日报称65星仅为其快照，不是成功验证。
53.1%为项目定义下的函数匹配率，24.21%为整函数匹配字节覆盖，不是完整原版EXE一致率；未独立复测。

## 来源

- [候选：资源日报介绍Redivivus与只读提案，2026-11-08 16:30:20北京时间](https://x.com/i/status/2119346771860349404)
- [补充README：固定窗口内2026-11-08 18:35:56提交，构建、通关与限制](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/README.md)
- [同提交CONTRIBUTING：Agent只读数据库、证据分级与提案审阅](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/CONTRIBUTING.md)
- [同提交BYTE-MATCHING：地址归一、分母与排除项](https://github.com/jaenster/redivivus/blob/bb149dcad7fd53c59f6d0d1d305a0f8656263a5f/BYTE-MATCHING.md)

[English](en/redivivus-diablo2-ghidra-agent-proposals.md) | [返回目录](../README.zh-CN.md)
