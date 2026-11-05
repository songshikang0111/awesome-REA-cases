# Claude Duet安装卡片：宝玉触发Skill安装后询问skill_propose机制

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-06
阶段：分析测试

2026年11月6日03:53:03（北京时间），宝玉（@dotey）介绍对Claude Duet的具体行为研究：为测试Skill如何安装，先在对话中提交一个Skill让其安装，看到安装更新卡片后，再问为何能安装并弹卡片、自己的项目如何做同样功能。作者称Agent会解释有skill_propose工具，并建议先让它写详细技术方案。

目标是研究并重建Agent产品的Skill安装交互，和此前Claude Design Skill输入输出风格重建是不同功能目标。先触发上下文再询问是作者方法，工具名称和内部机制仍是Agent／作者解释，未取得内部工具schema、服务端代码、权限校验或实际复刻实现；不把模型自述当源码真相。补取确认署名与两张附图存在，未完整验证图中技术方案或运行相同输入对照。analysis-test表示作者做过行为探查，不表示本合集复现，未提REA；未安装其Skill或修改任何Agent配置。

封存1赞、350浏览、0转发；工具机制是作者转述Agent解释，非独立内部实现审计。

## 来源

- [宝玉的Claude Duet Skill安装与skill_propose研究报告，2026-11-06](https://x.com/i/status/2118431419424714878)

[English](en/dotey-claude-duet-skill-propose-behavior-study.md) | [返回目录](../README.zh-CN.md)
