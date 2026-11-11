# 0sec Labs的0／0verse：连接Ghidra、angr与AFL++的AI安全研究框架

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-11
阶段：相关项目

2026年11月11日11:07:13（北京时间），Bobo（@okeyccronald）介绍0sec Labs开源AI安全框架0，称它不是模型，而是可接已有模型的控制层，提供本地Web控制台、无头CLI与MCP；二进制研究引擎0verse连接Ghidra、angr与AFL++，设置步骤会定位Ghidra／Java、安装Python分析依赖并检查反编译器。这里收录具体AI逆向工具相关项目，不把通用渗透宣传当已完成案例。

帖子列14个provider或Claude／Codex／Gemini CLI运行时、Apple Silicon macOS与Linux x64／ARM64和容器方案，称MIT OR Apache-2.0。发帖者说对照官方README与网站，但明确尚未hands-on；本合集也只补查原帖，没有读仓库、许可文本、实现、官方研究页或实际分析输出。这些接口、支持范围和许可均保持报道归因。

重要边界：研究预览不是生产就绪；默认shell在主机，须隔离不可信目标并配置scope插件，插件名称不构成沙箱保证。工具免费不等于模型免费，约每个XBOW题5.20美元是团队示例转述，不是本工具二进制任务的成本基准；团队页面30余个已合并Linux内核零日也不能证明由0／0verse发现。只研究获授权对象，未列具体逆向样本或复现结果。REA未提及，本合集未安装依赖、执行目标或扫描服务。

封存0赞、57浏览、0转发；来源自称对照官方不等于本合集审计或复跑。

## 来源

- [Bobo介绍0与0verse及未亲测、安全和费用边界，2026-11-11](https://x.com/i/status/2120352619826753760)

[English](en/0sec-zero-0verse-ai-binary-security-harness.md) | [返回目录](../README.zh-CN.md)
