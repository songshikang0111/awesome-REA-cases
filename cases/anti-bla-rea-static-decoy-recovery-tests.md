# Anti-BLA：为REA量出诱饵边界，四种自有样本不等于通破保护

分类：应用与客户端 · REA
记录日期：2026-11-10
阶段：分析测试

2026年11月10日18:16:07至18:16:12（北京时间），ShambaC（@shamba_c09）发布Anti-BLA，让Claude Code、Codex、Cursor及Gemini CLI在REA分析受阻时辨认BLA式诱饵，给出可追查的位置与下一步。两条候选为发布及集成说明，同串四条测试帖只是补充证据，不另作候选。npm元数据将anti-bla指向ShambaC/anti-bla并标MIT；补读固定c2edfa17a183cfcccedb5e2d20ca78e9ae1339b2的README与两份评测记录，提交于当日15:38:50，早于发布帖。记录日期为11月10日，不能仅据文档日期推定执行时刻。

真实BLA展示记录注明Windows 11 x64、Node22.21.1、REA6.8.0经MCP、BLA3.2.1、Anti-BLA0.1.0，单次、由实现Agent判分。JS许可样本从422B变135778B，REA保留1951未知项；辅助层称证明31个guard恒定、恢复五个拆分字符串。文档同时承认每个字符串可能有两个候选，不是所有运行值唯一确定，REA内部语义预算仍触顶。ASAR从1115B变18154053B；量得索引17443968B后只改受支持的asar.max_header_bytes并重试一次，恢复准入、识别notes:quota及桥接名，但REA结果仍partial。

WASM有251个导出却都指向同一9字节函数体，函数体由人手读；REA的WABT未配置，不可把缺provider写成这次实测被BLA打败。SQLite六表中五个诱饵、三个陷阱列，辅助层只认模式并找licenses，不读行值；REA因宿主Node版本而无provider，也未复现BLA原报告里的列求值错误。四个干净对照未报medium/high项，不等于任何干净应用零误报；四个加固样本合计不足1秒是辅助层耗时，不是端到端Agent逆向时间。76测试通过是发布者自述，本合集未运行。

较早的同日配对记录用Sonnet5.5，两臂各七问、非盲、一次、同一实现Agent判分。两臂都是17/17事实正确；REA单用77738 tokens、85369ms，配Anti-BLA为78790 tokens、88605ms，REA调用7降至2，并多一条不支持的额外说法。因此该试验没有准确率或token收益；样本小且可手读，多个provider缺失，不能当通用胜率。

项目称CLI不执行、修改或提取目标，不联网，skill指挥Agent而CLI自身不调用REA；只建议受支持设置及一次重试，不会解除REA内部预算，也不保证新混淆能检出。未审完源码、安装或复跑测试；本条记录可检查的作者测试及其限制，不是独立证明保护已被普遍击败。仅限自有或授权目标。

两候选封存分别0赞/3浏览/0转发与1赞/23浏览/0转发；不是成功率。
npm取阅latest为0.1.1，展示用0.1.0；版本不能混同。未下载包或执行样本。

## 来源

- [候选：ShambaC发布Anti-BLA，2026-11-10 18:16:07北京时间](https://x.com/i/status/2120098169698779194)
- [候选：REA上层集成、MIT与授权限制，2026-11-10 18:16:12北京时间](https://x.com/i/status/2120098189084856548)
- [同串补证：JS样本，2026-11-10 18:16:08北京时间](https://x.com/i/status/2120098173876396176)
- [同串补证：Electron样本，2026-11-10 18:16:09北京时间](https://x.com/i/status/2120098177680609455)
- [同串补证：WASM与SQLite，2026-11-10 18:16:10北京时间](https://x.com/i/status/2120098181472198891)
- [同串补证：测试与扫描耗时自述，2026-11-10 18:16:11北京时间](https://x.com/i/status/2120098185263960470)
- [补充固定README：提交2026-11-10 15:38:50北京时间](https://github.com/ShambaC/anti-bla/blob/c2edfa17a183cfcccedb5e2d20ca78e9ae1339b2/README.md)
- [补充固定真实BLA展示记录：记录日期2026-11-10](https://github.com/ShambaC/anti-bla/blob/c2edfa17a183cfcccedb5e2d20ca78e9ae1339b2/benchmarks/results/bla-showcase-2026-11-10.json)
- [补充固定配对试验：记录日期2026-11-10，无准确率或token收益](https://github.com/ShambaC/anti-bla/blob/c2edfa17a183cfcccedb5e2d20ca78e9ae1339b2/benchmarks/results/paired-2026-11-10.md)

[English](en/anti-bla-rea-static-decoy-recovery-tests.md) | [返回目录](../README.zh-CN.md)
