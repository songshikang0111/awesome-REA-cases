# Codex 0.169.0控屏架构：源码观察与闭源执行器转述分开看

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-28
阶段：分析测试

2026年11月28日10:08:18（北京时间）的长帖称阅读本地Codex 0.169.0源码镜像d32063f9，研究Computer Use为何少做逐次截图点击。作者的源码观察是Rust工具处理器不包含底层截图、点击、键盘执行器；models.json中除旧gpt-5.5外新模型采用code_mode_only及node_repl_disabled等开关；connectors按cua_repl／node_repl识别常驻REPL，通过nodeRepl.emitImage回传截图给云端模型，而非JS本地看图。批量异步JS可在必要节点才截图，是其解释的减少往返路径，不是实测提速。

帖子称开源Rust侧主要是安全壳：Windows应用白／黑名单按AUMID或发行者、产品、二进制名配置；Guardian为登录、敏感数据与权限等高风险操作另设审查模型，风险分级提示约11KB；截图与审查上下文隔离。作者另将闭源执行器的SkyComputerUseService、持久JS、macOS Accessibility／Windows UI Automation双通道及Mac后台／Windows前台差异归于社区拆解与文档反馈，未当作从该源码直接证明。

其复用idea是用持久JS、无障碍树、应用白名单与独立危险动作审查包装现成桌面驱动，而非搬走闭源二进制或复制GPT原生能力。未提供公开镜像链接、文件行号、原始社区来源、执行跟踪或基准，本合集未独立读取该版本、审闭源服务或执行客户端；具体模型、开关和平台差异均按作者报告。收录AI工具架构研究，不证明AI参与原始源码审读，REA未知。

候选封存16赞、358浏览、8转发、7回复；没有可复跑的性能对照。

## 来源

- [Codex 0.169.0 d32063f9源码与闭源控屏架构分析，2026-11-28 10:08:18北京时间](https://x.com/i/status/2126498386732056717)

[English](en/codex-01690-cua-repl-source-architecture-analysis.md) | [返回目录](../README.zh-CN.md)
