# 多阶段Windows下载器实习：用Claude Code分析，再对照LimaCharlie遥测

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-22
阶段：分析测试

2026年11月22日12:57:02（北京时间），《恶意软件教科书》作者吉川孝志（@MalwareBibleJP）介绍LimaCharlie提供的两小时免费工作坊。具体对象是面向Windows的多阶段下载器，学习目标是把AI辅助静态分析的预测变成可测试的检测与响应规则，而不是仅接受模型给出的解释。

据该帖，学员与Claude Code用LCRE做初筛、功能与指标梳理、外部工具信息补充，并可选用Ghidra反编译；随后将分析映射到MITRE ATT&CK，设计警告、停止与隔离等分阶段响应，再在装有LimaCharlie EDR的隔离Windows VM执行样本，对比实际遥测并调整误报。课程还要求辨别哪些AI结论需分析员判断。帖称浏览器内提供每人独立的Linux与Windows环境，由Claude远控Windows，学员不直接接触样本；实验VM免费，Claude订阅须自备，还需免费LimaCharlie账号与命令行基础，不要求既有逆向经验。

补取原帖确认署名及内容，但未取得课程原文、样本标识、模型回答、规则或执行日志。两小时是课程标称时长，不是已完成逆向工时；免费、隔离设计和验证流程均为吉川的二手课程说明，不证明学员都取得相同结果或环境绝对安全。本合集没有注册、下载或执行恶意样本，也未开VM或安装依赖；REA未提，按教学分析实验保留analysis-test，不把课程流程写成独立复现。

11月22日候选快照：4赞、521浏览、3转发、0回复；补取原帖赞数会变化，不覆盖封存快照。

## 来源

- [吉川孝志介绍Claude Code／LimaCharlie下载器工作坊，2026-11-22 12:57:02北京时间](https://x.com/i/status/2124366520776347715)

[English](en/limacharlie-claude-code-windows-downloader-workshop.md) | [返回目录](../README.zh-CN.md)
