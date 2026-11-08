# VerifiedIDA：给模型主导的IDA分析保存证据、修改回执与可恢复调查

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-07
阶段：相关项目

2026年11月4日23:47:26（北京时间），Ryan Naraine介绍SentinelLabs的VerifiedIDA，称其让LLM逆向可检查、可续做、可复用；23:57:10，SentinelOne官方账号确认项目归属与证据定位。补查找到SentineLabs/verified-ida，静态阅读固定提交caab127be22a071d93a9b4737ff65c39b57842c8的README、usage、worked-example与SECURITY。该提交时间为2026年9月15日01:19:07北京时间，早于本窗口，不把11月宣传当源码新发布。

项目要解决发现散落在对话、注释夸大代码含义、工具说成功却无法检查的问题。模型选择调查路线并提出命名、注释、接口与共享类型修改，host核对目标和当前证据，在候选IDB中应用并检查，记录ledger与回执，再把接受的变化纳入工作数据库。笔记本保留问题与进度；独立review需另行调用，并非analyze自动包含。可选coverage reconciliation默认关闭，也不要求所有函数都被标注。

项目ComRAT示例是已记录静态调查，未执行恶意软件：Sol从CreateProcessW参数的48字节偏移推导结构，在类型库创建SuspendedProcessContext后测得使用数0，再把函数参数改为结构指针后测得1，反编译显示ctx->process_info。保存后用新IDA进程重开检查，回执标verified；unknown_28仍未解释。这里只能支持项目所示类型编辑与持久化，不证明全部结构语义或恶意软件分析正确，review也可能漏错。本合集未重跑该记录。

支持环境为Linux、Python3.10以上、IDA Pro9.3及Hex-Rays，需自备许可证与模型访问，不能把MIT源码许可当免费IDA。文档称IDA worker禁网络、脚本在一次性数据库运行，样本不作为程序启动；控制器仍向模型商发送代码、结果和上下文，IDB含样本字节，不能称纯离线或天然安全。独立review默认预算250M记录token、2500请求、四活跃小时，不是本例实付成本；缓存计数和边界检查还可能越过token阈值。未安装依赖、运行IDA或获取样本。

2026年11月7日16:11:01的新日语转述补充实验性call-flow模式：函数结论确定前，先要求调查全部直接内部被调用函数。在ComRAT一个函数上，模型未被提示关键被调用函数，却检查20个直接被调用函数，找到前六次尝试均漏查的转发导出递归解析；但早期全局应用对8项编辑生成265个必查节点，因此缩小适用范围。转述还称主要以GPT-5.6 Sol评估，暴露误命名、发现未写入IDB、计划丢失和过早停止调查。未读该新文章或新版代码，不把这些数字当旧固定提交中已核验行为，也不将持久化检查等同语义正确。

封存候选：Ryan 1赞、142浏览、0转发；SentinelOne 0赞、97浏览、0转发。未以补取热度覆盖；verified为数据库修改验证，不是语义正确认证。
11月7日候选封存9赞、649浏览、1转发；20个被调用函数、六次遗漏、8编辑／265节点均为新二手转述，非独立复测。

## 来源

- [Ryan Naraine介绍VerifiedIDA，2026-11-04 23:47:26北京时间](https://x.com/i/status/2118007217647726704)
- [SentinelOne官方项目介绍，2026-11-04 23:57:10北京时间](https://x.com/i/status/2118009669239153074)
- [补充固定提交README，提交早于本窗口](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/README.md)
- [同提交ComRAT类型应用静态示例](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/docs/worked-example.md)
- [同提交使用、review与预算边界](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/docs/usage.md)
- [同提交隔离与模型数据传输说明](https://github.com/SentineLabs/verified-ida/blob/caab127be22a071d93a9b4737ff65c39b57842c8/SECURITY.md)
- [日语转述：ComRAT call-flow调查与范围扩张限制，2026-11-07 16:11:01北京时间](https://x.com/i/status/2118979524046278875)

[English](en/verifiedida-evidence-led-llm-reversing-harness.md) | [返回目录](../README.zh-CN.md)
