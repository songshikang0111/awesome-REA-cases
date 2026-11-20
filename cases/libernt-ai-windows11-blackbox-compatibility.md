# LiberNT：AI辅助Windows 11黑箱兼容研究，仍是测试用预发布系统

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-21
阶段：进行中

2026年11月21日02:18:46（北京时间），HKEPC（@hkepcmedia）介绍LiberNT这一以Windows 11兼容为目标的自由NT操作系统，转述AI帮助研究底层行为、编写和审查代码，并称团队要求人工审查与端到端验证。用途是在现代硬件上运行Windows应用，而非找回Windows原始源码。报道宣称132项性能比较中112项领先、个别超过2000%、弱项最多落后约28%；没有在此取得对应环境、原始结果或重跑，均不作为本合集性能结论。

补查公开仓库，阅读固定提交0542ae580c1d36b5fb226aa4cf9fdacce030cbdf的README与AGENTS。该提交的committer时间为11月19日02:58:01北京时间，早于本窗口；11月21日读取仅作项目身份、方法与限制补证，不是新增候选。README明确AI协助阅读文档、提取定义、把Microsoft Learn的规定与自己的函数行为作对照，并声称人工审查生成代码、合入前人工执行端到端测试。项目使用SDK／WDK头文件、Windows 11公开符号、微软文档和黑箱运行，要求逐项对照同一测试在Windows 11的结果；不将反汇编／反编译Windows代码直接转写为实现。规则不是逐次已执行测试的证明，本合集未检查完整测试日志或运行系统。

文档确认它是ReactOS分支，且大部分树仍共享；列出新的内存／缓存管理、ARM64、WoW64、图形和设备工作，不据媒体的全新核心表述宣称整套系统从零重写。README列amd64、arm64、riscv64镜像，i386源码构建；同一版本AGENTS仍把RISC-V64／PPC标为进行中，不能把镜像列表等同各架构功能完全对齐。发布页构建被明确标为测试用Debug预发布，不供依赖的日常电脑使用。报道中的REA名称未由文档确认是morluto/rea工具；归为other-ai、in-progress。没有下载镜像、安装依赖或运行目标，也没有独立验证兼容性、性能或法律合规。

候选封存12赞、844浏览、4转发、0回复；性能数字来自报道而非本合集测量。

## 来源

- [HKEPC的LiberNT报道，2026-11-21 02:18:46北京时间](https://x.com/i/status/2123843509157539992)
- [补充：窗口前11月19日02:58:01固定README，AI方法与预发布限制](https://github.com/LiberNT/LiberNT/blob/0542ae580c1d36b5fb226aa4cf9fdacce030cbdf/README.md)
- [补充：同一固定版本AGENTS，来源规则、ReactOS关系与Windows 11对照要求](https://github.com/LiberNT/LiberNT/blob/0542ae580c1d36b5fb226aa4cf9fdacce030cbdf/AGENTS.md)

[English](en/libernt-ai-windows11-blackbox-compatibility.md) | [返回目录](../README.zh-CN.md)
