# browser-capture：CY介绍把CDP流量与调用栈交给Agent的采集工具

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-25
阶段：相关项目

2026年11月25日02:00:02（北京时间），CY（@AIchanyi）介绍browser-capture，目标是让授权Web研究从看单次请求变成可回查证据链：经Chrome DevTools Protocol连接BitBrowser、AdsPower或Chrome／Chromium／Brave／VisibleV8，分stealth、standard、deep模式。帖子称基于Node.js22、无第三方依赖，有CLI与SKILL.md可接Claude Code／Codex；收集页面、iframe、Worker的静态与eval代码并以SHA-256去重，导出Wasm及导出表，采HTTP、WebSocket、SSE、NDJSON、DOM存储与crypto.subtle信息，响应体上限16MiB。

帖子另称默认不调用Runtime.enable，隐藏hooks；替换debugger保持原位置长度，支持本地override、最长32层异步调用栈关联与HAR1.2导出。这些是介绍者的功能主张，不是本合集审源码或验证反检测。未从短链取得仓库、版本、SKILL正文或具名采集样例；与XCrun旧Web skill没有确认的实现关系，不能借用其作者归属。

声称CDP／浏览器API只连127.0.0.1或localhost，不证明浏览器不访问外网、采集内容不落盘或无泄密风险；其列举的cookie、存储与响应可能含敏感数据。本合集未连接浏览器、抓账户流量、安装依赖或运行代码。保留相关研究工具，不能说抓到的源码等于恢复服务端实现；未提REA。

候选封存1赞、34浏览、0转发、0回复；所有功能、限制与依赖均为转述，没有实现或抓取核验。

## 来源

- [CY对browser-capture与Agent技能的完整介绍，2026-11-25 02:00:02北京时间](https://x.com/i/status/2125288347731906893)

[English](en/browser-capture-cdp-agent-reverse-engineering-tool.md) | [返回目录](../README.zh-CN.md)
