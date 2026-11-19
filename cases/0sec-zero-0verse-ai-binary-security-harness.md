# 0sec Labs的0／0verse：连接Ghidra、angr与AFL++的AI安全研究框架

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-20
阶段：相关项目

2026年11月11日11:07:13（北京时间），Bobo（@okeyccronald）介绍0sec Labs的0：它不是模型，而是接已有模型的安全研究控制层，提供本地Web、无头CLI与MCP；二进制引擎0verse连接Ghidra、angr和AFL++。介绍列14个provider或Claude／Codex／Gemini CLI、Apple Silicon macOS、Linux x64／ARM64和容器，称MIT OR Apache-2.0。Bobo明确未hands-on，功能与许可保持转述归因。

11月20日01:46:27（北京时间），美濃加茂まむ（@superdoccimo）补充Plan、Discover、Attack、Triage、Verify、Report流程，称Verify用独立会话重跑候选，每项最多5轮，证据从candidate到impact-proven分级；0verse的本地MCP暴露9项工具。补取原帖全文获得候选结尾未列全的内容，但这仍不是本合集审计实现或运行验证。

新帖列CVE-2026-68124的Linux MCTP串行驱动零长帧缓冲区溢出、CVE-2026-63801的TIPC异步解密use-after-free等，称由0sec自动工具发现。本合集没有读取CVE原始条目、补丁或复现日志，不能把团队工具归因缩小为由公开0／0verse二进制链路发现。帖中XBOW 93／95、黑盒并集81／104、冷跑45／104、Cybench36／40与npm审计F1为自报或转述，不是pass@1；没有将其变成本工具的通用成功率。

重要边界仍是研究预览、默认主机shell、须隔离不可信目标和限制授权范围；scope插件名不是沙箱保证，免费工具不等于免费模型，每个XBOW题约5.20美元也不是二进制任务成本基准。尚未读官方源码、许可文本和研究页，未安装依赖、执行目标或扫描服务；REA未提，保留related-project。

11月11日候选封存0赞、57浏览、0转发；11月20日候选1赞、233浏览、0转发、0回复。来源称对照官方不等于本合集审计或复跑。

## 来源

- [Bobo介绍0／0verse及未亲测、安全费用边界，2026-11-11](https://x.com/i/status/2120352619826753760)
- [美濃加茂まむ补述复核流程、证据等级和自报结果，2026-11-20](https://x.com/i/status/2123472988192276897)

[English](en/0sec-zero-0verse-ai-binary-security-harness.md) | [返回目录](../README.zh-CN.md)
