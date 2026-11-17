# OpenConche：AI参与研究四款Chocolatier游戏，以新引擎运行原始资产

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-17
阶段：待验证

2026年11月17日11:00:39（北京时间），The Gaming Emporium（@McGroin83）介绍open-conche的OpenConche v1.1，称AI Agent广泛参与逆向、实现、审阅和测试，目标是让2007至2009年的Chocolatier经营游戏在Windows、Linux和macOS运行。补取完整帖后定位公共仓库，并阅读固定提交f82158242e44ad0d55b0ac1dd61ee48fd75c0403的README；提交时间为11月14日06:37:12北京时间，属于窗口前补充证据。

项目README明确称用几周AI驱动开发研究原游戏二进制与脚本，重写C++20／SDL3引擎；docs/re保存事实文件，docs/design记设计理由，但本合集未逐份审这些研究文件或源码。四个支持对象是Chocolatier、Chocolatier 2: Secret Ingredients、Chocolatier: Decadence by Design及The Great Chocolate Chase。前三款来自Big Splash Games，外传由Zemnott开发、PlayFirst发行，不能把四款全归Big Splash。它们共用一个引擎项目，不拆成四个独立案例。

作者动机是现代macOS不能运行旧程序、Windows显示驱动兼容问题，以及原800×600画面放大效果差。README称字体按原生分辨率绘制，但美术仍为原分辨率缩放；内置游戏选择器，游戏存档独立于原版，第三代与Reforged内容也分开。原始资产必须自备，MIT只覆盖新引擎，不分发或重新授权原作。作者明确是爱好项目、无路线图或维护支持承诺，其他PlayFirst游戏不会自动兼容。

帖子称v1.1，但未核release标签、平台构建、完整流程测试或图像一致性；未下载二进制、资产、依赖或运行游戏，未查看截图。AI型号与REA使用未指定，几周为作者粗略开发周期，不是可迁移工时。保留公开文档支持的项目报告与unverified状态。

候选封存2赞、238浏览、0转发、0回复；读取文档不等于复现四款游戏或核实v1.1发布。

## 来源

- [The Gaming Emporium介绍OpenConche v1.1与AI参与，2026-11-17 11:00:39北京时间](https://x.com/i/status/2122525293185302820)
- [窗口前补充：OpenConche固定README，2026-11-14 06:37:12北京时间提交](https://github.com/open-conche/OpenConche/blob/f82158242e44ad0d55b0ac1dd61ee48fd75c0403/README.md)

[English](en/openconche-chocolatier-ai-engine-reimplementation.md) | [返回目录](../README.zh-CN.md)
