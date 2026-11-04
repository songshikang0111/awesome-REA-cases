# FVCOM海洋模型：转述Gemini/Antigravity用59分钟重建Rust核心

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-04
阶段：待验证

2026年11月4日09:23:30（北京时间），viest（@viest_w）转述Google材料Modernizing 40-year-old scientific code with Gemini 4 Argon：Antigravity/Gemini追踪FVCOM海洋模型Fortran90/C的全局变量与求解循环，生成六部分蓝图后重建Rust核心，解决科学代码移植的数值保持问题，不是无源码二进制反编译。

帖称原库264文件174774行；11分钟建gfortran基准、3分钟分析、45分钟实现13个各不足240行的模块。约束为禁止unsafe、热循环零堆分配、每文件不超400行、分支覆盖至少95%和100种子对拍。报告六个老bug；首轮37测试有一项浅水单层网格越界，修后42测试全过、覆盖96.8%，误差3.91×10⁻¹³；883ms降到469ms（称1.88倍），11.84MB降到5.48MB，另做LLVM PGO并称公开/migrate-to-rust Skill。

均为帖子转述自测，未核查原博客全文、代码、硬件、规模或全部失败记录。核心不等于174774行全库，近似数值一致不等于字节零差异或物理正确。模型名、59分钟、bug数与开源状态未独立确认；未运行目标、安装依赖或执行Skill，REA未提及。

候选快照3赞、221浏览、0转发；补取确认账号，不是实验验收。

## 来源

- [viest转述FVCOM核心Rust迁移，2026-11-04](https://x.com/i/status/2117789802431226036)

[English](en/fvcom-gemini-antigravity-rust-core-migration-report.md) | [返回目录](../README.zh-CN.md)
