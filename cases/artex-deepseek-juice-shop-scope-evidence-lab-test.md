# ARTEX研究自有Juice Shop：DeepSeek报10条finding，范围门控仍需网络隔离

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-24
阶段：分析测试

2026年11月24日11:29:53（北京时间），@pingfengjj以长文记录自有Ubuntu服务器上的ARTEX分析测试。目标是自己启动、仅在容器网络可达的OWASP Juice Shop Web靶场，不是任意互联网站点。作者报告平台planner拆intent，三worker调用真实工具，fact／finding与资产、探索图关联；本机OpenAI兼容网关接deepseek-v4-pro。它是具体AI辅助应用安全与行为分析实验，未说明REA，也不等于恢复Juice Shop全部源码。

作者称约27分钟任务done、判定目标达成，输出10条finding（2 critical、4 high、4 medium），覆盖8类，任务token为In 4.2M／Cache 4.0M／Out 121k。文章说每条有命令与观察到的响应，靶场日志还显示一个SQL注入挑战解锁；这些为作者自报，图片和原始日志未在此检查，且其后明确承认两个intent重复报同一购物车IDOR，因此10条不等于10个独立漏洞或新CVE。Cache可能与输入口径重叠，不擅自相加成总token。

更有价值的限制是作者读源码后发现target gate只拦平台自有HTTP工具，Bash中直接调用扫描器不受此门控，因此另加容器网络硬隔离、任务scope和审批。记录这一边界不代表在此已审计实现；本合集没有设置防火墙或测试网段。原文还说默认流量录制为空，本次证据是finding中的文本命令与响应，不是完整代理抓包；正式报告需人工去重。源码构建约20多分钟、镜像约7.5GB是部署自述，不是逆向工时或性能基准。

文章链接BaaRai/ARTEX，但未在此读其源码、验证与原作者仓库的关系、构建镜像或复跑漏洞。与既有ARTEX活体协议、Android调查及固件项目是不同目标，单列Juice Shop授权靶场分析测试；不提供对生产系统的攻击流程，保持analysis-test与作者结果归因。

候选封存0赞、42浏览、0转发、0回复；27分钟、10条／8类及token均为作者报告，存在重复finding且不是独立复现。

## 来源

- [pingfengjj的ARTEX／Juice Shop部署、门控边界与测试自述，2026-11-24 11:29:53北京时间](https://x.com/i/status/2125069366018584763)
- [文章指向的公开ARTEX fork；未读取源码或运行](https://github.com/BaaRai/ARTEX)

[English](en/artex-deepseek-juice-shop-scope-evidence-lab-test.md) | [返回目录](../README.zh-CN.md)
