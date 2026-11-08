# Discord新客户端mod想法：社区预期用AI研究Rust版再做插件

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-07
阶段：待验证

2026年11月5日07:15:01（北京时间），kingsoul（@voidheartly）预期AI会加快Discord新客户端逆向，mod很快跟进。旧补查父串指向Wumpus Central当日06:22:56关于Rust／GPUI的社区消息，以及旧mod依赖Chromium注入可能失效的讨论。未取得官方声明，不把全面替换Electron／React Native、约290MB对此前2GB的内存说法当事实。07:45:40的另一评论预期更好、更快的Rust mod；两人不因同一目标成为开发团队。

11月7日12:40:06的候选在回复中写出更具体的拟议Claude指令：监听Discord API的新版本发布，启动子Agent反编译二进制、重映射函数、修补mod，运行单元与集成测试，再推送修复。其用途是客户端更新后自动维护自己的mod，不只是首次重建。这里只记录idea，没有启动监听或Agent，也没有把引号中的命令当作实际发生。

没有客户端修订、二进制、扩展接口、mod功能、仓库、已运行监听器或测试日志。旧帖的很快和更快不是工时或基准；新管线也未证明能可靠映射函数、自动通过测试或获授权分发。仍为unverified，未提REA，未运行Discord或注入客户端。

两条旧候选封存依次1赞／99浏览／0转发、0赞／12浏览／0转发；未把父串传播量当idea热度。
11月7日候选封存2赞、61浏览、0转发；监听与测试管线是拟议指令，不是执行日志。

## 来源

- [候选：kingsoul预期AI加快Discord新客户端逆向，2026-11-05 07:15:01](https://x.com/i/status/2118119859653619727)
- [候选补证：Rust mod与性能预期，2026-11-05 07:45:40](https://x.com/i/status/2118127573117059226)
- [补充会话根：Wumpus Central的Rust／GPUI客户端消息，2026-11-05 06:22:56](https://x.com/i/status/2118106749446103371)
- [新增idea：Claude监听Discord版本并反编译、重映射与测试mod，2026-11-07 12:40:06北京时间](https://x.com/i/status/2118926444986540171)

[English](en/discord-rust-client-ai-reversing-mods-idea.md) | [返回目录](../README.zh-CN.md)
