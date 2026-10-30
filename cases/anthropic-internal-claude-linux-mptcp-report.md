# Linux MPTCP：二手报道内部Claude模型研究内核网络竞态链

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-30
阶段：分析测试

2026年10月29日09:33:04（北京时间），Ummon在五目标报道中转述Anthropic的Linux网络栈研究。演示目标是暴露多路径TCP监听器的内核路径，报道概括竞态导致释放后使用、泄漏内核地址后影响回调控制流，声称无需凭据或用户交互达到root命令执行。只记录研究层面，不给触发包、利用代码或操作步骤。

此前补读10月27日官方文章，确认项目自述约48分钟取得地址、再五分钟达到命令执行，失败竞态只使握手失败而不使系统崩溃。官方标识CVE-2026-98432，称上游及维护中的稳定分支已修复；时间不是通用成功时长，监听配置也不能扩大成所有Linux均远程可达。内部模型未具名，从人工初始提示开始；协调披露与未报告在野利用不等于没有攻击者。

10月30日11:31:02新候选中，SANS.edu Internet Storm Center（@sans_isc）以同一CVE报道Claude发现Linux内核MPTCP RCE。按相同目标追加，未把播客标题当新漏洞。补查CVE Program记录：首次公布10月15日，当前记录10月30日02:08:12Z更新，属于较早披露及本日文档补证，不是本窗口首次发现。Linux CNA标题为在RCU宽限期后释放inet_opt/ireq_opt，记录IPv4 TCP选项生命周期的释放后使用和补丁引用；底层缺陷不是只限MPTCP。

另读oss-security在10月30日08:21:41北京时间转发的Go安全团队原信（原信10月30日07:34:28北京时间），两者早于此候选；信引用Anthropic演示，明确已展示RCE需要MPTCP监听，但不能排除非MPTCP系统的类似攻击。Go1.24起Linux监听socket默认启用MPTCP，可被逐socket设置覆盖。团队强调升级已修复内核才是最佳修复，逐程序禁用MPTCP是脆弱缓解，不是彻底修复。这里不提供攻击方法，也不对具体读者主机作暴露判断。

本次已核对CVE与安全公告的存在及范围，修正此前完全未查公告的限制；没有核对每个稳定分支构建、复跑利用或评估现实受影响主机数，不能把公告存在当独立复现。保留分析测试状态，REA未提及。本合集仅静态阅读公开文字，未向目标发包。

较早共同候选快照0赞、157浏览、0转发；48分钟与五分钟为项目演示。
CVE及Go公告已静态核对，不等于逐分支构建、利用或影响范围独立验证。
SANS候选快照1赞、446浏览、1转发；CVE文档与原信早于候选，不增加新候选数。

## 来源

- [Ummon完整报道中的Linux MPTCP研究，2026-10-29](https://x.com/i/status/2115617884533907835)
- [补充原始研究：10月27日Anthropic Linux章节](https://www.anthropic.com/research/discovering-vulnerabilities-with-claude#5-zero-click-remote-code-execution-in-linux)
- [SANS Stormcast以同一CVE报道Claude/Linux研究，2026-10-30](https://x.com/i/status/2116009959230234650)
- [补充CVE Program记录：IPv4 TCP缺陷与补丁引用，首次公布10月15日](https://cveawg.mitre.org/api/cve/CVE-2026-98432)
- [较早补证：Go安全团队原信的oss-security转发，MPTCP范围与升级建议](https://www.openwall.com/lists/oss-security/2026/10/30/1)

[English](en/anthropic-internal-claude-linux-mptcp-report.md) | [返回目录](../README.zh-CN.md)
