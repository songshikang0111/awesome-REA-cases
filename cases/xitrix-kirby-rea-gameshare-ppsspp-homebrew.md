# Kirby到PPSSPP：XITRIX用REA研究GameShare启动调用

分类：游戏与游戏保存 · REA
记录日期：2026-11-20
阶段：待验证

2026年11月20日05:03:05（北京时间），XITRIX（@X1TRIX）解释自己的PPSSPP Switch 2移植如何加入GameShare。PPSSPP是PSP模拟器；作者说先用REA研究一款Kirby游戏如何通过系统SDK启动该功能，再从homebrew调用相同API。研究目标是复用系统分享能力，不是恢复整个Kirby源码，也未指明系列中的哪部作品。

补读同串11月20日03:21:50的介绍，作者称移植使用kaiHEN，GameShare会创建第二个PPSSPP实例，交给客户端Switch控制，使朋友可从同一收藏玩PSP游戏或一起本地联机。这条介绍早于本轮04:00窗口，只作用途与结果背景，不计候选。另一参与者说libounce已有GameShare API；XITRIX随后称自己也写了SDK，这只是作者说法，不把两套实现当作相互验证。

本轮已核对对话署名和上下文，未阅读API实现、SDK或完整REA会话，未观看演示或测试主机，不能确认兼容机型、网络限制或每款游戏的联机表现。旧Kirby进行中记录来自另一作者，且未指明作品；没有同项目证据，不把它的进度与账号担忧并入本条。保留为未独立验证的具体互通成果报告。

候选封存1赞、163浏览、0转发、1回复；不是项目总热度。

## 来源

- [XITRIX解释REA研究Kirby的GameShare SDK调用，2026-11-20 05:03:05北京时间](https://x.com/i/status/2123522473777885254)
- [补充背景：PPSSPP Switch 2移植与GameShare双实例，2026-11-20 03:21:50北京时间，早于本轮窗口](https://x.com/i/status/2123496993884660100)
- [补充：XITRIX称也制作了SDK，2026-11-20 05:35:14北京时间](https://x.com/i/status/2123530566104703355)

[English](en/xitrix-kirby-rea-gameshare-ppsspp-homebrew.md) | [返回目录](../README.zh-CN.md)
