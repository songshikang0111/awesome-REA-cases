# Mario Kart 64原生PS3移植：既有反编译、Claude协作与作者实机调试

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-11
阶段：进行中

2026年11月11日16:30:17（北京时间），yibie清单介绍Mario Kart 64 on PS3，称既有反编译在PSL1GHT上运行、仓库不带游戏资产、运行时从用户ROM加载，并有具名AI披露。它不同于Mario Kart Wii、网页MK64或MK8 Deluxe项目。

补充读取stingziz0u/mk64-ps3固定提交32602e5f01dd71820e1174ebde7ff10351ab4fe8的完整README，提交于11月11日10:44:01北京时间，早于本轮窗口，属于补充文档而非新候选。文档明确建立在n64decomp/mk64既有反编译之上，不能把手工上游工作归为AI从零完成。AI disclosure称作者与Claude实时协作多个会话，所有测试和调试由作者在真实硬件完成；这是项目自述，不是本合集实机复现，REA未提及。

文档列原音频引擎48kHz、720p缩放、4:3／16:9、一至四人DualShock3、30帧或插值60帧及计时赛ghost的Controller Pak模拟。60帧插值不是原生游戏逻辑稳定60帧的测量。数据型Mod通过从ROM重建599张表支持；代码／汇编hack不支持，约190张只读表未重建，重排布局的ROM可能加载后仍失败。仓库还描述qemu PowerPC hosttest，但未读取测试输出。须自备合法USA ROM；本合集未下载游戏资产、构建或运行PKG。

清单整体2赞、249浏览、0转发；7星、953文件是清单转述，未独立计数，不表示游戏完成率。

## 来源

- [yibie的MK64 PS3项目转述，2026-11-11 16:30:17北京时间](https://x.com/i/status/2120433924434452690)
- [补充项目README及AI disclosure，固定窗口前2026-11-11 10:44:01北京时间提交](https://github.com/stingziz0u/mk64-ps3/blob/32602e5f01dd71820e1174ebde7ff10351ab4fe8/README.md)

[English](en/mario-kart64-ps3-psl1ght-ai-port-report.md) | [返回目录](../README.zh-CN.md)
