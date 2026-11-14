# LASIK：静态清除BLA诱饵，2100万到1.7万是读入量估算而非Agent实测

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-11
阶段：分析测试

2026年11月11日08:00（北京时间），TechVerser（@realfxw）介绍LASIK（LLM Agents Sight In Kode），称morphh7用Claude Code编写去混淆pass、边界测试和MCP服务，帮助AI读懂经BLA（Blind LLM Agents）反Agent保护的程序。本轮查到公开仓库pktq/lasik，固定提交58f47e047a4d858e29186e5c3dab38ebba8a7786，提交时间11月10日08:20:52北京时间，早于候选窗口；它是补充项目材料，不是本窗口新提交。帖子中的morphh7与仓库账号不同，未独立确认身份对应或AI开发会话。

目标不是重建某个商业应用，而是从受保护发布物中去掉不透明条件、不可达诱饵、附带密钥的字符串编码、部分完整性互锁、二进制填充与诱导模型的文本，再让REA等工具读取清理副本。README提供CLI、MCP、库与Agent skill，声明不执行输入；这不等于能保证任意敌意文件绝对安全，也不恢复已经销毁的名字、注释或源码。它与既有Anti-BLA恢复实验是不同项目。

补读固定README与benchmark：项目在公开BLA CrackMe v6—v9共15文件上报告估算读入量21,104,859到16,718 token，约1262倍缩减；其中WASM按解压大小计数。文档明确用代码约4字符／token、hex/base64约2字符／token、二进制1字节／token估算，不是实际Agent或REA运行，更不是实付成本、准确率或破解成功率。另对21种格式各一个自有小样本用BLA3.2.1加固，报告默认及全opt-in两组均21/21 healed，分别11与10文件恢复字节一致。healed并不意味着每份输出字节一致；这类小样本不能代表真实大型应用。

README对BLA3.2.2列59/63 shield文件完全处理，JS／HTML与native仍为部分覆盖；Go、Flutter、Bun、BEAM、APK/DEX及IL2CPP还含从BLA源码生成的fixture边界。本合集阅读soundness.test.ts，见保留参数写入调用、JSX组件、var提升、超范围整数、别名修改、页面全局与自有完整性检查等回归断言。它们支持项目承认并防范误删的事实，不是本合集重跑，也不是对任意变换的外部形式证明。候选称12处误删与README称两次独立审查，均保留为项目／报道归因，未独立审计。未下载或执行目标、安装项目依赖或运行LASIK；未将CrackMe可读性等同于已求得密钥或flag。

候选封存0赞、5浏览、0转发；补查原帖确认TechVerser署名，不用随后增长的浏览量替换封存快照。
固定提交日期2026-11-10T00:20:52Z；文档与测试是窗口前补证，没有在本合集执行。

## 来源

- [候选：TechVerser介绍LASIK与Claude Code开发，2026-11-11 08:00北京时间](https://x.com/i/status/2120305505465979321)
- [补充固定README：用途、覆盖及限制，提交2026-11-10](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/README.md)
- [补充固定benchmark：估算方法与21格式自有样本](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/docs/benchmark.md)
- [补充固定回归测试：曾改变行为的反例与断言，仅静态阅读](https://github.com/pktq/lasik/blob/58f47e047a4d858e29186e5c3dab38ebba8a7786/tests/soundness.test.ts)

[English](en/lasik-bla-static-deblinding-cli-mcp.md) | [返回目录](../README.zh-CN.md)
