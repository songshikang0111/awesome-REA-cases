# LEGO Island：Claude署名提交与三文件字节一致重建报告

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-19
阶段：待验证

2026年11月19日16:30:13（北京时间），yibie介绍isledecomp/isle的LEGO Island反编译，称最近30条提交有68处Claude trailer。目标是重建1997年游戏英语1.1版，供理解、修改与后续移植，不是AI从零创作一个新游戏。

补读固定提交fc9cc83ebea6a434ba7e172a96e1c4280afbd860的README；提交日期11月16日04:18:52北京时间，早于窗口。项目称CONFIG.EXE、ISLE.EXE、LEGO1.DLL全部反编译，用原Microsoft Visual C++ 4.2及ReproBit冷重建三者字节一致，另以reccmp逐函数比较。普通CMake开发构建不属于精确发布认证；此仓库只面向32位Windows，跨平台另在isle-portable，运行需自备游戏文件。

补读9月8日05:04:53北京时间的提交14dd37b，带Claude Fable 5.1共同署名与会话链接，描述新增三目标冷重建CI。另一9月10日23:00:49北京时间提交563915f描述用函数记录替代117处overlay改动；AI署名证明具体贡献归因，不代表整个多年项目由AI完成，也不意味着唯一原始源码恢复。未将候选的68处trailer当68个独立贡献者或测量工作量；未复核该总数。README与提交信息已读，完整ReproBit报告、CI实际结果和源级真实性未审，也未构建；字节一致保持项目自报unverified，未确认REA。

## 来源

- [yibie列LEGO Island与Claude提交署名线索，2026-11-19 16:30:13北京时间](https://x.com/i/status/2123333006870131110)
- [补充LEGO Island固定README，提交2026-11-16 04:18:52北京时间](https://github.com/isledecomp/isle/blob/fc9cc83ebea6a434ba7e172a96e1c4280afbd860/README.md)
- [补充Claude署名：加入ReproBit三目标冷重建CI，2026-09-08 05:04:53北京时间](https://github.com/isledecomp/isle/commit/14dd37baefec418246c61eec6038dcfb3b97e8c1)
- [补充Claude署名：替换overlay为函数记录，2026-09-10 23:00:49北京时间](https://github.com/isledecomp/isle/commit/563915fbff5c07e612ff9afe46e6d0635e840b3c)

[English](en/lego-island-claude-credited-reprobit-decompilation.md) | [返回目录](../README.zh-CN.md)
