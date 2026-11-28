# 冷启动退全屏：Gemini分析metadata与汉化DLL的修复转述

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-28
阶段：待验证

2026年11月28日09:40:00（北京时间），JJBond（@JJBondBuilds）转述一名网友让Gemini修复游戏bug：据称模型解析global-metadata.dat，把冷启动必现的退出全屏定位到汉化插件version.dll，再自行写补丁、备份、重装并重启验证，问题消失。这里收录的是利用既有游戏元数据与插件调查兼容性故障的具体案例，不把一句“游戏逆向了”扩成恢复整部游戏源码。

原帖未命名游戏、引擎版本、汉化包来源、模型版本或补丁细节；global-metadata.dat这一文件名不替代目标确认。补查只确认转述者和图像附件，未读截图内容、原始对话、反汇编或冷启动回归记录。修复成功仍是二手报告，不能据此保证跨版本有效、插件安全或自动操作全程正确。本合集未下载DLL、执行补丁或运行游戏，未确认使用REA。

候选封存7赞、728浏览、1转发、6回复；未得到原始补丁或独立测试。

## 来源

- [JJBond的Gemini／global-metadata.dat／version.dll修复转述，2026-11-28 09:40:00北京时间](https://x.com/i/status/2126491263604257201)

[English](en/gemini-unity-versiondll-fullscreen-localization-fix.md) | [返回目录](../README.zh-CN.md)
