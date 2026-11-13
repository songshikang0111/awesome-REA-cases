# ZigZag与Brother Skitch：从ChatGPT直连转述补到公开实现，协议复用Respira

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-13
阶段：待验证

早期资料为2026年10月26日20:36:06（北京时间）汉卿（@hanqing1120）的12美元硬件订阅回复，以及同日18:26:52的Valar（@ValarMind）父帖。后者称Kath Korevec购入约300美元Brother刺绣机，用ChatGPT制作直连程序，把生成图案做成布贴；每月12美元、售罄和作者任职均为该转述，不是独立核实。旧记录将其称作OpenAI产品负责人，现补查公开GitHub个人资料显示simpsoka自称Kathy Korevec、Product @google；纠正此前将二手职务写得过实的问题，不以当前资料反推历史任职。

本窗2026年11月13日09:15:25，Andrew111（@AndrewSignalZ）明确介绍开源Zigzag、simpsoka/zigzag仓库及300美元绣花机替代订阅软件的用途，并转述Show HN的314分、130评论及二手设备约100美元。这些仍是帖子说法，未读HN原串或核验价格，不能称本合集可复现或设备恢复了全部功能。按同一作者线索与Brother直连目标补充既有ID，不另建重复案例；早期资料不作为本窗新候选重审。

补充读取固定提交7fdb49f34517f569128bf02f215b45fa280c818c的README和NOTICE，提交时间为11月13日08:50:47北京时间，属于项目补证而非第二候选。README将目标明确为Brother Skitch PP1：Rust刺绣编辑器将SVG转成针迹，导出PES/DST/EXP/JEF/VP3或蓝牙直传；MCP让Claude Code、Codex等在可见设计上操作，也可发送设计和读取机器状态。文档报告Mac/Windows发布路径，但本合集未下载安装包或审实现。暂停仍需机器本体按键，不能通过蓝牙暂停；设置写入尚等待确认布局及原值写回一致，不称全设备控制。

关键归属更正：NOTICE明确Brother PP1蓝牙协议、缝制流程、错误及断线回退、PEN编码等移植自Jan-Henrik Bruhn的Respira（Apache-2.0）；PES/PEC/DST布局来自pyembroidery，Image Trace等来自VectorCraft。不能把整套协议发现归给ChatGPT或ZigZag作者独立完成。MCP支持证明项目面向AI设计工作流，不证明早先ChatGPT如何参与协议研究，二手AI归因仍未获得原工作日志。

README自报136项库测试、153项编辑器/MCP测试、所用Image Trace的222项测试；文件写出经pyembroidery读回针迹一致，并称在真实Skitch PP1测试。它们是项目声明，未读取逐项日志、观看演示或重跑；模拟机器测试不等于每种真实设备通过。保留unverified，未运行代码、连接设备或确认订阅条款和保护绕过；REA未提及，不与Brother扫描按键NAS项目合并。

早期候选快照1赞、16浏览、0转发；300美元、每月12美元及售罄是二手说法。
11月13日本窗快照1赞、118浏览、0转发、2回复；HN314分／130评论及约100美元为转述，未核原串和价格。
136／153／222为固定README各测试组自报数量，不是本合集执行结果；协议与PEN等移植归属见NOTICE。

## 来源

- [早期来源：汉卿的12美元订阅回复，2026-10-26](https://x.com/i/status/2114697580362055944)
- [早期父帖：Valar的Kath Korevec／Brother／ChatGPT转述，2026-10-26](https://x.com/i/status/2114665054780133816)
- [本窗Andrew111明确Zigzag仓库的二手报道，2026-11-13 09:15:25北京时间](https://x.com/i/status/2121049262045937692)
- [补充固定README：Skitch PP1、MCP及项目自测，2026-11-13 08:50:47提交](https://github.com/simpsoka/zigzag/blob/7fdb49f34517f569128bf02f215b45fa280c818c/README.md)
- [同提交NOTICE：Respira协议移植及其他上游归属](https://github.com/simpsoka/zigzag/blob/7fdb49f34517f569128bf02f215b45fa280c818c/NOTICE)
- [补充公开GitHub个人资料：Kathy Korevec的自述，非历史任职证明](https://github.com/simpsoka)

[English](en/kath-korevec-brother-chatgpt-embroidery-report.md) | [返回目录](../README.zh-CN.md)
