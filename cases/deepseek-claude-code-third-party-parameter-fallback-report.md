# Claude Code第三方接口：DeepSeek逆向的参数降级转述，非降智动机铁证

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-02
阶段：待验证

2026年11月2日20:33（北京时间），AI Fun（@ai_funss）转述用DeepSeek逆向Claude Code，调查第三方API接入后的能力变化。帖称第280101行在thinking／effort被拒后移除深度思考重试；网关对私有参数返回400时，经Latch机制依次放弃深度思考、结构化输出、1M上下文与Threads，不向用户提示。

正文称“降智铁证”，但没有版本、文件路径、对应代码、参数名、请求响应或复现实验。行号不能定位版本；回退若存在，也不能仅由参数不兼容推导恶意动机或推理质量下降。补取原帖确认署名及附图存在，未读图片或取得原分析。保留为第三方适配机制调查转述，不将四阶段顺序或全体模型受影响写成事实。REA未提及；未访问网关凭据或运行客户端。

候选快照11赞、5139浏览、1转发；280101行、1M及四阶段降级均为未核实转述。

## 来源

- [AI Fun转述DeepSeek调查Claude Code回退，2026-11-02](https://x.com/i/status/2117233546020667885)

[English](en/deepseek-claude-code-third-party-parameter-fallback-report.md) | [返回目录](../README.zh-CN.md)
