# Xenosaga Trilogy Port：Claude辅助整合PS2反编译到Linux，第三部仍未开放

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-28
阶段：进行中

2026年11月28日19:51:11（北京时间），The Gaming Emporium介绍xenosagaport的Xenosaga Trilogy Port：把PS2三部曲整合为一个Linux启动器和AppImage，称使用Claude Code辅助开发。

补读固定5e3b605eef3cbda937aed0775efa87cc3cf42d4d README，提交2026年11月28日11:28:36 UTC、早于候选且在本轮窗口内。作者明确移植、启动器和工具由Claude／Claude Code辅助，基础是OpokXeno的三部反编译，并称上游亦用AI。第一部自报可玩，第二部可玩但仍有问题和测试，第三部尚未来临；Windows只是计划。文档列真16:9、第一部速度与战斗动画跳过、Event Theatre、可选HD包和跨部共享记忆卡，不能据一个统一启动器认定三部全完成。

须自备合法NTSC-U光盘镜像，不需要BIOS。构建与发布检查声称从用户盘读取所需VU微码、检查hash及32字节以上共享片段，并允许源码显式表格或通用库表格等例外；这是项目流程，非本合集验证无版权字节。README还承认上游反编译当时无license文件，不将开放代码升级为任意再许可授权。没有GitHub Actions构建，因为匹配PS2构建需要游戏数据。仅阅读文档，未下载游戏、发行包或运行测试；几周开发为作者估计，不是测得工时。

候选快照1赞、37浏览、1转发、0回复；可玩性均是项目报告。

## 来源

- [The Gaming Emporium的三部曲移植介绍，2026-11-28 19:51:11北京时间](https://x.com/i/status/2126645074289205710)
- [窗口内候选前固定README：AI归属、分部状态与许可／数据检查边界，2026-11-28 11:28:36 UTC](https://github.com/xenosagaport/xenosaga-trilogy-port/blob/5e3b605eef3cbda937aed0775efa87cc3cf42d4d/README.md)

[English](en/xenosaga-trilogy-linux-claude-opokxeno-port.md) | [返回目录](../README.zh-CN.md)
