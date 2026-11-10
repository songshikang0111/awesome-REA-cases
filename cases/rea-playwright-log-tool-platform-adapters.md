# log客户端适配：matt用REA与Playwright观察Instagram，再查公开客户端

分类：应用与客户端 · REA
记录日期：2026-11-10
阶段：进行中

2026年10月23日09:37:13（北京时间），matt（@matthewsoldit）称把自己的log工具重做为原生Codex插件、Claude connector并支持Claude Duet，以REA与Playwright观察内部API，计划下周测试后推main。避免平台自动活动信号、基本不会烧账号是当时作者的推断，不是已验证的账号安全保证。本轮回查旧原帖只用于确认与新帖同一作者、同一log项目，不重新审判旧候选。

2026年11月10日06:19:44的新候选补充具体用途：log是跨X、Slack、Discord与Instagram的消息和联络工具，作者希望个人AI拥有分散在各平台的上下文。其自述适配流程是经MCP请求新平台，生成骨架并在AdsPower浏览器打开；REA与Playwright观察按目标完成的操作并记录步骤，再分析JS bundle中实际内部调用的名称、作出文档，用GitHub API按调用名找相近客户端，比较提及程度与目标功能后纳入项目并配置schema。作者明确说亲眼看到AI对Instagram完成这件事；这只是一次集成自述，不证明所有平台所有调用都能被发现或任何账号长期不受限。

作者描述本地消息索引用BM25、all-MiniLM-L6-v2、HNSW与reciprocal rank fusion；发送前另用jina-embeddings-v5-omni-small与jina-reranker-v3.5挑相关上下文，图像／视频由本地LFM2.5-VL-450M描述，语音由AssemblyAI转录、Inworld TTS生成并回听。帖列twikit、instagrapi、endcord、gabriel客户端与curl_cffi及chat-xdk，称消息存入SQLite并通过平台WebSocket送到Claude Code。这些是架构清单，不是本合集确认各库兼容、解密正确、数据全本地或端到端隐私；外部转录与语音服务尤其不能因本地索引而省略。

帖前半的沟通分析涉及20073条本人消息、约5700万token；草稿检查另称用66116条消息与130条规则，两个语料口径不同。rapport是拟建的一人一档关系评分延伸，作者明说尚未建成，不另当已交付产品，也不把个人沟通百分比当客户端恢复准确率。

补取完整新帖与旧帖确认署名及项目连续性，没有访问消息或账号。未读取确切仓库、许可、代码、适配记录、输入输出或回归测试；免费开源是作者说法，不能核实旧下周推main的计划已完成。保留进行中，不提供规避检测或访问他人账号的方法；API可观察及找到公开客户端均不意味着获得自动调用或数据处理授权。本合集未运行浏览器、客户端、模型或任何目标。

原始发布日期2026-10-23 09:37:13，北京时间；旧补审来自08:00至12:00窗口。
旧下周测试与推main为计划；避免账号封禁说法仍未验证。
11月10日候选封存0赞、130浏览、0转发；20073条／约5700万token与66116条／130规则是不同自报统计，未复算。

## 来源

- [往期候选：log工具、REA/Playwright与下周测试计划](https://x.com/i/status/2113444602808250641)
- [新候选：matt的Instagram适配流程、log架构与未建rapport，2026-11-10 06:19:44北京时间](https://x.com/i/status/2119917883535040608)

[English](en/rea-playwright-log-tool-platform-adapters.md) | [返回目录](../README.zh-CN.md)
