# CLI-Anything：从源码生成Agent命令行层，补充运行与遥测边界

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-28
阶段：相关项目

2026年11月22日00:14:26（北京时间）的中文帖子介绍HKUDS CLI-Anything，为Blender、GIMP、FreeCAD、Obsidian与LibreOffice等软件加命令行，避免Agent依赖截图点击。它描述七步流水线：扫源码、定命令分组、生成带REPL／JSON及撤销重做的Click CLI，再测试、写文档、发布并产出SKILL.md。这里的研究对象是可读源码与软件操作接口，不是已证明能通吃闭源二进制。

帖子称调用真实后端，并转述2461个测试、Blender208个测试、FreeCAD258条命令、火星车建模和四分钟画HTTPS图等演示；没有取得仓库测试输出、命令列表或演示记录。61868星与热榜第三只是帖子当时宣称，未独立核验。作者同时提醒依赖强模型、无源码时质量下降、常需refine多轮。

2026年11月25日14:25:49，Felix（@Stevezh1f）补充介绍现成cli-anything-hub与自行生成harness两条路线，明确自己未亲测。他转述需要目标源码和本机真实应用，强模型示例为Claude Opus 4.6、Sonnet 4.6与GPT-5.4，弱模型可能产出不全或错误CLI，通常要多次refine；Python需3.10以上，Windows用Claude Code需Git for Windows含bash或WSL，生成消耗模型额度。帖子还称cli-hub默认向PostHog发匿名事件，可用CLI_HUB_NO_ANALYTICS=1关闭，并提醒Agent接真实软件后会执行命令，须限定授权。这些是具体部署／隐私边界的转述，不是本合集验证过遥测开关或完整支持。

Felix引用11月24日20:06观察的1075当日新增星与约6.42万累计星，说明当日按UTC且未结束，并称Apache-2.0；未独立复查。按AI分析与Agent互通的相关项目收录；安装和生成指令未执行，未核完整软件支持、测试通过或二进制恢复。模型名是帖子工作流背景，不是本合集模型测试；未确认使用REA。

11月22日候选封存2赞、300浏览、0转发、8回复；仓库星数及测试数量未复查。
11月25日候选封存1赞、33浏览、0转发、0回复；引用的星数快照在11月24日20:06，不是11月25日实测。
2026年11月28日11:36:45新介绍称registry约79个CLI、第三方约24个，README的30套harness合计2464测试全通过，含真实应用端到端测试；这是其读仓库后的转述，不是本合集复跑，也不是所有约103个入口都验收。具体用途包括GIMP批量滤镜、LibreOffice真实PDF导出、Calibre电子书转格式、Kdenlive／Shotcut剪辑、VideoCaptioner字幕及FreeCAD火星车／杀戮尖塔2演示；软件本体必须安装，各CLI实际覆盖以各自说明为准。强调Python3.10以上、Windows Git bash或WSL、强模型和多轮refine，只有二进制时效果变差；CLI可执行命令读写本地文件，第三方registry须审来源。Apache-2.0、arXiv报告、约6.67万星及668当日星为帖子说法，未另查；没有新代码、测试日志或遥测开关验证。封存1赞、65浏览、0转发、1回复。

## 来源

- [HKUDS CLI-Anything七步流程与局限的中文介绍，2026-11-22 00:14:26北京时间](https://x.com/i/status/2124174608618168350)
- [Felix补充源码／运行环境、模型与PostHog遥测边界，2026-11-25 14:25:49北京时间，明确未亲测](https://x.com/i/status/2125476030005526899)
- [registry、真实后端用途、30套harness测试与二进制局限的新介绍，2026-11-28 11:36:45北京时间](https://x.com/i/status/2126520645353611557)

[English](en/cli-anything-source-analysis-agent-cli-pipeline.md) | [返回目录](../README.zh-CN.md)
