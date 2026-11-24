# Hellcats Over The Pacific：Matyo用Claude与Godot重建1991年Mac飞行游戏

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-24
阶段：进行中

2026年11月24日14:45:35（北京时间），Matyo（@matyo91）介绍重建Hellcats Over The Pacific，一款1991年的Macintosh空战模拟游戏。他称几个月前开始研究档案，现已在Godot运行并提供浏览器演示入口；还研究过历史1.0.3、1.0.4及Leyte Gulf扩展。补取原帖全文确认署名与末尾内容，演示未打开。

作者把ResEdit与Ghidra用于资源提取和Motorola 68000汇编反编译，Claude Code按其提示分析、重建逻辑并生成C与GDScript，Godot负责历史环境重建与现代平台适配。他称自己没有亲写代码，但负责理解架构、定义方法、拆问题、指导Agent并检查结果；不能改写为无人工参与或AI独立恢复原源码。

作者区分三条路线：Original重建68k、内存和Macintosh Toolbox环境；Native逐步迁入Godot原生组件；Enhanced面向Android／iOS等现代设备且仍验证中。项目明确仍在重建，不把浏览器可启动的报告推广为全游戏完成、各历史版本一致或手机可玩。未取得仓库、许可证、资源来源、差分测试、帧率或完整通关记录，未运行演示、下载游戏或执行代码。REA未提，保留进行中与作者自述边界。

封存1赞、19浏览、0转发、0回复；无亲写代码及浏览器运行均为作者报告，未取得独立测试。

## 来源

- [Matyo的Hellcats重建路线与Claude Code归因，2026-11-24 14:45:35北京时间](https://x.com/i/status/2125118617742094763)

[English](en/hellcats-matyo-claude-godot-macintosh-reconstruction.md) | [返回目录](../README.zh-CN.md)
