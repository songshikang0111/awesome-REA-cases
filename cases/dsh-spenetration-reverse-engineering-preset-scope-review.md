# DSH渗透与逆向预设：CyHawk质疑默认授权，后续版本加入范围门禁

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-20
阶段：相关项目

2026年11月20日19:27:09（北京时间），CyHawk Africa（@CyhawkAfrica）介绍对suixin406/dhs-spenetration的审查：为DeepSeek Harness提供渗透与逆向Agent预设，称56个skills、49篇知识材料、命令行工具与自动决断，担忧只要用户给出IP、域名或URL就视为获授权。它是工具与安全边界研究，不是本合集已验证的入侵案例。

补读候选前最近提交3bfd9e6290c47797e1b3eb25ff732b5f29101029（11月20日17:12:45北京时间）的README与PROMPT，旧提示确实声明用户提供的目标一律视为授权且不另询问。README头部称48篇正文，知识库章节又写49篇，不能无口径地都当正文数；56技能与六CLI也是项目声明。与逆向直接相关的是静态／动态分析与协议还原技能、前端bundle接口提取、APK字符串提取、加密／签名研究，未运行这些工具。

补充当日19:54:10提交c4f4ca5da1c9075090b239b8f04e9cd430e2203a的README与PROMPT时，项目已经声明74技能、48篇正文和六CLI，要求AUTHORIZED-TARGETS.json、匹配主机／端口／动作／时间／授权依据，默认拒绝，破坏性动作每次另确认。它晚于候选，作为版本变化补证，不冒充候选已报告；不能断言此变化由CyHawk引起。

旧版有直接文本证据支持审计担忧；新版有门禁设计不代表每条Agent路径已强制执行或生产安全。没有审完整代码、运行单元测试、安装依赖或探测任何目标，也未验证所有技能或数量。只记录文档与版本差异，不传播攻击操作；REA未提及，状态related-project。

候选封存0赞、27浏览、1转发、0回复；56／74技能、48正文／49材料依不同版本和口径记录，不是独立盘点。

## 来源

- [CyHawk Africa审查DSH预设与授权问题，2026-11-20 19:27:09北京时间](https://x.com/i/status/2123739921210876383)
- [补充：候选前17:12:45版本README](https://github.com/suixin406/dhs-spenetration/blob/3bfd9e6290c47797e1b3eb25ff732b5f29101029/README.md)
- [同版PROMPT：提供目标即授权的文本](https://github.com/suixin406/dhs-spenetration/blob/3bfd9e6290c47797e1b3eb25ff732b5f29101029/PROMPT.md)
- [补充：候选后19:54:10版本README，默认拒绝门禁设计](https://github.com/suixin406/dhs-spenetration/blob/c4f4ca5da1c9075090b239b8f04e9cd430e2203a/README.md)
- [同一后续版本PROMPT：范围登记与动作门禁要求](https://github.com/suixin406/dhs-spenetration/blob/c4f4ca5da1c9075090b239b8f04e9cd430e2203a/PROMPT.md)

[English](en/dsh-spenetration-reverse-engineering-preset-scope-review.md) | [返回目录](../README.zh-CN.md)
