# Craft Anything：Rust研究与重建工作台，项目自报检查仍有边界

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-02
阶段：进行中

2026年11月2日09:51:48，Smartpig（@Smartpigai）介绍Craft Anything，让AI研究网站、应用或游戏后建新项目并对照修改；11:15:23，明子206（@mingzi206）进一步宣传全量自动Hook、符号执行架构图和几分钟完成。按项目名补查storytold/craft-anything公开仓库，读取固定提交32b80be89061896921d370e8f4f952ab707e2270的README与STATUS。提交时间为当日11:40:37北京时间，STATUS标11月2日；其中10月18日实跑和10月23日审计是较早项目记录，不是本窗口的新实验。

项目称纯Rust引擎提供314个CLI／MCP工具，其中298个属引擎，桌面界面与Agent共用研究、构建、检查、迭代流程。默认Clean room只看访客可见界面、用户图片与描述，拒绝内部读取；Deep允许代码、文件、网站JavaScript与可选Ghidra。建造优先调用用户自己的Claude Code，分析可接API或本地兼容服务；Codex适配器存在但尚未在真实安装中验证。Clean room是项目模式名，不是本合集对净室合规或法律安全的认证。

STATUS自报10月18日Windows headless实跑：网页96%相似度、1.5分钟；小桌面应用9分钟，但仅以构建检查；Rust游戏到Build即停止、未到Check。网页相似度是项目检查指标，不等于功能等价。文档还说明游戏self-test由生成物自己报告，尚未独立观察游戏过程或测量其数值；运行研究只启动原应用一次采窗口和UI树，不持续操控，Frida会话工具部分模拟，Clean room完整构建尚无实跑。这些具体边界不支持候选“记录所有系统调用／内存迁移”“几分钟完成任意克隆”等泛化。

README称early alpha并区分已做与部分完成，安装包说明不作为本合集实际下载或跨平台测试记录；本文只阅读公开文档与提交元数据，没有执行目标、构建仓库、安装依赖或重跑作者测试。与ArtCraft应用套件的Adobe归因争议分开记录，不因同组织而认定该套件此前逆向了Adobe。

候选封存快照：Smartpig 8赞、692浏览、2转发；明子206 2赞、59浏览、0转发。
314工具、96%、1.5分钟、9分钟及审计测试为项目口径，未独立复现；Codex实装、Clean room实跑与部分动态分析待验证。

## 来源

- [候选：Smartpig介绍Craft Anything流程，2026-11-02](https://x.com/i/status/2117072151476080832)
- [候选补证：明子206的Rust／动态观察宣传，2026-11-02](https://x.com/i/status/2117093182441972165)
- [补充项目README：固定提交，2026-11-02](https://github.com/storytold/craft-anything/blob/32b80be89061896921d370e8f4f952ab707e2270/README.md)
- [补充项目STATUS：含10月实跑与11月2日边界，固定提交](https://github.com/storytold/craft-anything/blob/32b80be89061896921d370e8f4f952ab707e2270/docs/STATUS.md)

[English](en/craft-anything-agent-study-rebuild-compare-report.md) | [返回目录](../README.zh-CN.md)
