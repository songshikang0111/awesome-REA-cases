# augur v1：字符串关联伪代码与缓存，报道保留IDA版本变化的性能边界

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-17
阶段：相关项目

2026年11月17日06:37:01（北京时间），吉川孝志（@MalwareBibleJP）整理Hex-Rays的三工具v1介绍，称augur提取字符串和关联函数伪代码，与haruspex一样输出结构体、枚举等类型，供后续静态工具与LLM研究，再由人验证。augur通过重用结果避免重复反编译同一函数；报道列开发者MacBook Air M3处理36个AArch64 ELF二进制，从39.3分钟缩到124秒。

补读Marco Ivaldi的Hex-Rays作者文章，发布2026年11月12日19:52:28 UTC，及augur固定9178c4e README，提交11月16日09:11:12 UTC，均为窗口前补证。文档确认先反编译全部函数以恢复更多字符串，再按字符串组织引用函数与类型头文件；反编译基于haruspex API。文章确认36个文件共2.2MB，从无既有IDB开始、计入初始分析，旧v0.9.3／IDA 9.3对新v1.2.0／IDA 9.5；作者强调数字同时包含工具与IDA升级，少字符串引用的二进制可能付出预先全函数反编译成本，不能保证一律更快。

文章描述LLM进一步初筛、人工静态动态确认，并称Claude帮助写测试；LLM更紧密集成与LibAFL自动确认仍在计划。没有逐样本核验或独立复跑，伪代码候选不是已确认漏洞，性能不能全归缓存或模型。同帖haruspex与rhabdomancer分别记录，不复制性能到它们。已读原帖、作者文章和固定README，未审完整源码或日志，未运行工具；REA未提及，保留related-project。

同一三工具候选封存4赞、414浏览、1转发、0回复；36个文件与性能数值来自项目作者测量，经候选转述并补读原文，未独立核验。

## 来源

- [吉川孝志转述Hex-Rays三工具v1，其中augur缓存与版本受限比较，2026-11-17 06:37:01北京时间](https://x.com/i/status/2122458950763499685)
- [窗口前补证：Marco Ivaldi作者文章与36文件组合版本基准，2026-11-12 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [窗口前补证：augur固定README，提交2026-11-16 09:11:12 UTC](https://github.com/0xdea/augur/blob/9178c4e9546a80ac2342625fa2049cbd2fcb156b/README.md)

[English](en/augur-ida-string-pseudocode-cache-tool.md) | [返回目录](../README.zh-CN.md)
