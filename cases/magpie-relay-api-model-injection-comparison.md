# Magpie中转API：Tmr比较三个模型追查prompt与tool注入

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-18
阶段：待验证

2026年11月18日20:09:07（北京时间），Tmr（@tmr11235）把一个未具名中转站接入Magpie，让Agent检查API是否有问题。目标是理解中转服务如何改写模型请求，而不是恢复某个模型权重。

作者称gpt-6.2-sol与claude-sonnet-5-5约四分钟结束，发现prompt注入并探出部分system prompt；gemini-4-argon花二十分钟，进一步指出混用的反代渠道、分别如何注入prompt／tool及注入内容。这些是作者的模型名称、耗时与覆盖比较，不是受控基准或独立确认中转站确实恶意。

补取原帖确认署名与文字。没有API地址、请求响应、注入原文、模型运行设置或验证日志，不能证明所谓全部内容恢复正确，也不能归纳模型排名。未请求该API、访问凭据或运行目标，REA未提及。

候选封存0赞、107浏览、0转发、1回复；四分钟与二十分钟为作者自述。

## 来源

- [Tmr的Magpie中转API模型比较，2026-11-18 20:09:07北京时间](https://x.com/i/status/2123025709744771253)

[English](en/magpie-relay-api-model-injection-comparison.md) | [返回目录](../README.zh-CN.md)
