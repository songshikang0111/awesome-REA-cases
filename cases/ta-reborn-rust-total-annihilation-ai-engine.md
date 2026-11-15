# TA Reborn：Claude参与的Rust横扫千军新引擎，复用自有游戏数据而非重编译原EXE

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-15
阶段：进行中

2026年11月15日16:30:12（北京时间），yibie（@yibie）介绍TA Reborn为Rust从零重写的新引擎，并指出credits列Claude Opus为开发。目标是用现代引擎读取玩家合法持有的1997年Total Annihilation（横扫千军）单位、地图和战役，不是恢复原始源码或重编译EXE。与基线Go语言的Nanolathe是不同仓库和实现，不因同一原游戏合并。

补读Jared-woodruff/TA-Reborn固定49186900c846f875c628eada350fc07b8d5dc62e README，提交2026年11月15日11:39:28 UTC，在候选之后但仍在本窗口内，仅作补证，不增加候选。文档将Jared Woodruff列为项目负责人、Claude Opus5.5为DEV、GPT6 Astra为QA，感谢社区数十年的格式研究；净室是项目自称，不是本合集审计。它描述HPI／GAF／3DO／COB等格式、COB脚本虚拟机、30Hz定点模拟、wgpu渲染与自己的lockstep联机。

同页宣传两万单位、战役、Mod、重放和多平台包；本合集没有测量帧率、验证完整战役或检验兼容性。文档明确不能与原版玩家联机，测试遇不到原游戏安装会跳过相关数据测试，因而通过基础测试也不能推出完整游戏等价。README展示当前开发构建并链接1.0.6发行，不把所有开发功能当成该发行已验证。

候选的2071文件未独立清点，不从文件数推断工作量。项目要求自备游戏，不提供原单位、地图、音画；原创引擎称GPLv3或以后，音乐另有权利，开源不使原游戏免费。本合集未下载游戏或发行包、未构建或运行，也未检查全部提交以量化AI贡献，REA未提及，保留进行中及项目自报边界。

候选整帖8赞、533浏览、0转发、7回复；2071文件为介绍者口径，未清点。
两万单位、30Hz与1.0.6为项目文档口径，非本合集性能测试；AI署名不是贡献比例。

## 来源

- [yibie介绍TA Reborn的Rust新引擎与Claude归属，2026-11-15 16:30:12北京时间](https://x.com/i/status/2121883453767688434)
- [候选之后的固定README补证：架构、credits与限制，提交2026-11-15 11:39:28 UTC](https://github.com/Jared-woodruff/TA-Reborn/blob/49186900c846f875c628eada350fc07b8d5dc62e/README.md)

[English](en/ta-reborn-rust-total-annihilation-ai-engine.md) | [返回目录](../README.zh-CN.md)
