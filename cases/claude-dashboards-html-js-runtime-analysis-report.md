# Claude Dashboards机制拆解：Rabi称模型写HTML／JS，读者侧runtime渲染

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-03
阶段：分析测试

2026年11月3日22:57（北京时间），Rabi Shanker Guha（@rabi_guha）称团队拆开研究Claude Dashboards，并把它与ChatGPT对比：Claude写原始HTML和JavaScript，但不直接填写数值，而是写一次连接逻辑，由runtime为每个读者渲染，不再调用模型。逆向目标是AI产品中生成代码、数据绑定与阅读时执行的分界。

补查原帖确认署名，未取得链接文章正文、捕获的代码、网络追踪或可复核实验。模型不写数字、每个读者不再调用模型均是作者概括，不能推断所有仪表盘、刷新、权限和数据源都免模型费用或完全本地。帖子未说明拆解是否由AI辅助，更未说明REA；按相关AI产品机制分析记录，标unknown，不猜工具。未登录产品、执行生成代码或检验与ChatGPT的比较。

11月3日候选快照10赞、362浏览、3转发；只取得摘要，未取得代码与调用追踪。

## 来源

- [Rabi Shanker Guha报告Claude Dashboards机制，2026-11-03](https://x.com/i/status/2117632138564821137)

[English](en/claude-dashboards-html-js-runtime-analysis-report.md) | [返回目录](../README.zh-CN.md)
