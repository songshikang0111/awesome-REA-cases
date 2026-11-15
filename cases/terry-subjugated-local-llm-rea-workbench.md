# Subjugated：Terry把本地LLM接入游戏REA工作台与Haiku任务队列

分类：应用与客户端 · REA
记录日期：2026-11-16
阶段：相关项目

2026年11月16日02:34:01（北京时间），Terry（@Cardgames）介绍自制本地LLM harness Subjugated的三种运行方式：独立CLI做测试、聊天、小研究；Gamedev Workbench独立窗口中的CLI处理Claude拒绝的工作；作为Haiku子Agent下面的SubSub agent，让Haiku排队和组织本地模型。

作者明确把游戏REA研究列为第二种用途，并提到清理provenance data等敏感任务；这里只记录用途归因，不提供去除来源记录的方法或认定这是合法必要步骤。帖子没有游戏名、输入、具体逆向产物、模型、版本、仓库或执行日志，不能宣布某款游戏已完成恢复。

作者称大量输出短摘要、Yes／No、Pass／Fail或测试编写运行的任务适合该架构，不适合复杂推理，并将组合质量比作Sonnet、称前沿模型200k Token任务可降到15k。没有任务、计数基线、价格或质量评估，这些是个人口径而非受控性能或成本测试。补取确认作者及文字，未运行harness、调用子Agent或测试游戏，以明确游戏REA用途的相关项目收录。

候选封存1赞、95浏览、0转发、0回复；200k到15k及Sonnet质量未独立测量。

## 来源

- [Terry的Subjugated三模式、游戏REA用途与Token自述，2026-11-16 02:34:01北京时间](https://x.com/i/status/2122035406715678884)

[English](en/terry-subjugated-local-llm-rea-workbench.md) | [返回目录](../README.zh-CN.md)
