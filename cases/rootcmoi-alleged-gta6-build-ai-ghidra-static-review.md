# 224GB所谓GTA VI构建的静态调查：rootcmoi承认用AI，也遭全量分析质疑

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-28
阶段：分析测试

2026年11月28日06:59:25（北京时间），@dddisasteroIogy引用rootcmoi的调查，讽刺“Ghidra＋已筛完224GB”只是问了Claude。07:42:04另一候选回复rootcmoi，建议IDA并警告不要完全相信Claude，尤其不能把224GB二进制当作已全部分析。两条是批评与建议，不是新的实测，也不证明作者实际使用IDA或Claude确实看完全部文件。

为确认目标，补读窗口外03:49:01的原帖：@rootcmoi声称对所谓GTA VI Xbox build的224GB、109个文件做只读研究，未执行二进制。报告主EXE约120MB、内含Flash／ActionScript 3及疑似Scaleform痕迹，一个像EXE的.bin实为不含可执行代码的Xbox目录，一DLL的CreateRemoteThreadEx只向自身进程建线程；12个Microsoft DLL的Authenticode摘要与内嵌签名不符，来源仍不明。EXE内时间戳为2026年11月13日22:40，不是本合集确认的构建发布时间。作者称在已分析范围没发现malware、infostealer或C2，同时明确不保证安全。

同窗口07:15:29作者在争论中解释，自动化了PE解析与完整性检查，再在Ghidra深入部分问题，也使用AI；未在该回复命名模型，Claude归因来自评论者，不能统一写成已核实工具会话。补充原帖只作目标与发现背景，不冒充本窗口新候选。没有文件hash、完整脚本、反汇编记录或可核样本，build真实性、签名异常原因及安全结论均未证实。本合集未取得、分发或运行疑似泄露游戏文件，不把静态未检出当安全认证，REA未提及。

候选06:59快照0赞、31浏览、0转发、2回复；07:42快照0赞、6浏览、0转发、0回复。批评互动不是分析结果验证。

## 来源

- [窗口候选：对Claude／Ghidra与224GB筛查的批评，2026-11-28 06:59:25北京时间](https://x.com/i/status/2126450851577257989)
- [窗口候选：建议IDA并质疑Claude全量分析，2026-11-28 07:42:04北京时间](https://x.com/i/status/2126461584776347732)
- [补充原帖：静态调查的范围与发现，2026-11-28 03:49:01北京时间，早于严格窗口](https://x.com/i/status/2126402936490139648)
- [补充作者回复：PE解析、完整性检查、Ghidra与AI，2026-11-28 07:15:29北京时间](https://x.com/i/status/2126454896484327877)

[English](en/rootcmoi-alleged-gta6-build-ai-ghidra-static-review.md) | [返回目录](../README.zh-CN.md)
