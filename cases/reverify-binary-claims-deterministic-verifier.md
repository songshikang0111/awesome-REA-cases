# Reverify：让工具检查Agent对二进制的猜测，97%不是所有模型错误率

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-23
阶段：分析测试

2026年11月23日18:42:13（北京时间），候选介绍2akouwu/reverify，用Propose→Verify→Evidence流程减少AI逆向中的字段、偏移和函数行为幻觉，并把上下文持久化。补读公开README和BENCHMARK.md，固定提交f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923（2026-09-07T10:12:05Z，窗口前材料）：CLI／MCP接收声明，通过真实文件的解析、反汇编、匹配或仿真，返回VERIFIED、REFUTED或INCONCLUSIVE及证据。另有源码等价比较与跨会话ledger／rollover设计，均为项目功能描述。

必须收窄候选的97%说法。BENCHMARK写明把教科书式push rbp；mov rbp,rsp序言当先验，盲套71个Windows11 x86／x64文件；69个不符，错误声明误放行为0，反馈一轮后重述观测指令71／71。它不是对某个在线模型71次独立问答，更不是AI普遍错误率。参考记录日期为2026-09-04，reverify0.10.0、Python3.14、capstone＋lief；零误放的95%上界仍为5.1%。

文档还报告三平台CI与aarch64外部运行，并承认macOS universal文件仍取x86_64切片等边界。本合集只读文档，未核原始逐文件记录、CI工件或外部复现，未执行二进制、仿真或模型。确定性验证也只检查所给声明及引擎覆盖，不是完整源码或语义等价证明；REA未提。

候选6赞、453浏览、0转发、4回复；1351星为帖子快照，不是本合集实测。
69／71、零误放与71／71为项目序言先验基准，不是通用准确率。

## 来源

- [候选介绍Reverify，2026-11-23 18:42北京时间](https://x.com/i/status/2124815780789534878)
- [补充README，固定2026-09-07T10:12:05Z提交](https://github.com/2akouwu/reverify/blob/f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923/README.md)
- [补充基准方法与边界，同一固定提交](https://github.com/2akouwu/reverify/blob/f32ea84ccd6bb2aff90eca711ccfdbf04e6b8923/BENCHMARK.md)

[English](en/reverify-binary-claims-deterministic-verifier.md) | [返回目录](../README.zh-CN.md)
