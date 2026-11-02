# knife：Dopax转述面向Agent的Rust多格式静态分析工具箱

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-02
阶段：相关项目

2026年11月2日09:24:17（北京时间），Dopax（@tensorstaff）在五项开源盘点中介绍knife：Rust终端优先的逆向工具箱，以CLI、TUI和MCP连接Agent，覆盖PE／ELF／Mach-O／Wasm静态分析，并称可审计缓解措施、追踪危险API与输出伪代码。它解决的是将二进制研究能力交给终端用户与Agent的问题，不是某个应用已完成的重建。

补查原帖确认归属，再按名称找到bl4ckr0ss3/knife，读取固定提交f260b87ffc54ae5c8c56cc31351334d209228745的README；提交为10月16日04:25:49北京时间，是窗口前文档，不是11月2日新实验。文档称静态读取目标不执行，MCP给Agent使用同一分析引擎，另有可接本地或兼容API的调查桌。它明确Wasm没有lifter、代码视图拒绝，直接调用图未覆盖间接分发，因此空结果不证明不可达；伪代码未建模部分原样显示。读取文档不等于审计实现、安全或恢复准确率。

384星是报道者标为截至11月2日的GitHub API口径，未独立核对，不视为实时热度。未运行仓库或样本、不保证所有格式功能相同或漏洞发现有效。REA未说明，MCP适配也不证明全部研发由AI完成。与同帖RDX独立建条；SkillOpt、Ethproofs与solOS并非此条逆向项目。

候选快照0赞、21浏览、0转发；384星为报道者11月2日口径，未独立核实。

## 来源

- [Dopax五项盘点中的knife介绍，2026-11-02](https://x.com/i/status/2117065226063667699)
- [窗口前补充：knife固定提交README，提交2026-10-16北京时间](https://github.com/bl4ckr0ss3/knife/blob/f260b87ffc54ae5c8c56cc31351334d209228745/README.md)

[English](en/knife-rust-static-analysis-mcp-secondary-report.md) | [返回目录](../README.zh-CN.md)
