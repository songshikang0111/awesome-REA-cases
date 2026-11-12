# Shape JavaScript虚拟机：BottingRocks发布AI辅助开发的Rust逆向工具包

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-12
阶段：待验证

2026年11月12日12:59:08（北京时间），BottingRocks（@BottingRocks）宣布开源Shape Security逆向工具包。目标是Shape的JavaScript虚拟机与其产生的请求信号，作者称研究始于数年前，近期很大一部分开发由AI coding agents加速；未指明模型或REA，不把多年研究全部归功于AI。

作者报告工具主要用Rust编写，包括VM字节码反汇编与分析、JavaScript自动去混淆、执行追踪与程序重建、信号提取及编解码、SDK与可复现实例，并称有跨数千seed的回归测试。作者强调真正的工作还包括理解系统、重建行为与验证正确性；这些是作者的实现和测试报告，不是本合集重跑。

补查公开BottingRocks/Shape固定提交ffce7d0cc06333ccdf36614f52abfb741a7c0e5f的README，提交于同日12:50:35，早于候选。文档描述解析捕获的JavaScript／WebAssembly、追踪Rust中间表示恢复可读程序，以及CLI和Node.js／TypeScript、Python、Go、Rust、C SDK共用引擎。它明确要求artifact与站点、构建、会话匹配；运行时值可能让追踪停止，输出应检查complete／stopped及unidentified、ambiguous、refused诊断。解出字段不保证任意修改都可重新编码，不支持的编辑会拒绝。因此不写成跨站点通用破解或全部行为已经恢复。

本合集仅静态阅读README的功能与限制部分，没有核回归语料、测试日志、完整实现或法律授权，也未下载目标脚本、捕获请求、生成或提交信号。数千seed仍只归因原帖。研究工具的公开存在不证明在任何生产服务上通用有效，保留unverified。

候选封存20赞、628浏览、1转发、0回复；数千seed为作者自报回归范围，没有本合集独立运行结果。

## 来源

- [BottingRocks发布Shape逆向工具包及AI参与说明，2026-11-12 12:59:08北京时间](https://x.com/i/status/2120743172813029407)
- [补充固定Shape README，2026-11-12 12:50:35北京时间提交，早于候选；静态核定位与限制](https://github.com/BottingRocks/Shape/blob/ffce7d0cc06333ccdf36614f52abfb741a7c0e5f/README.md)

[English](en/bottingrocks-shape-security-rust-ai-toolkit.md) | [返回目录](../README.zh-CN.md)
