# Instagram Reels：sujal称Claude研究APK后，用Java把入口弹回信息流

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-01
阶段：待验证

2026年11月1日21:45:02（北京时间），sujal（@sujshr）称自己整天刷Instagram Reels，于是用Claude逆向Instagram：手机通过USB调试连接、提取APK，然后用约30行Java，让点击Reels立即回到信息流。作者称不需root、不使用修改版App，并附视频与开源链接。保留为针对现有App行为的个人干预自述，不是重建Instagram或服务端推荐算法。

补读原帖与作者串。23:10:08，Gagan（@gagu_sh）提醒：如果以无障碍服务运行，就可能看到屏幕内容，应将服务限定到Instagram包，并检查没有记录或发送事件；23:11:56作者答复会研究和阅读。该条件式安全建议不能证明实现确实使用无障碍服务，更不能证明范围已收紧。

本合集未取得可明确归属的源码仓库，未读取该Java实现、检查权限、观看视频或在手机上测试。30行、立即弹回、无需root和开源均为作者报告；APK版本、具体识别机制、误拦截与跨版本兼容未知。未提REA，也不把这种干预写成平台认可、隐私审计通过或能彻底阻止短视频。

候选快照2赞、62浏览、0转发；约30行是作者代码量说法，不是本合集计数。

## 来源

- [sujal的Instagram／Claude与Reels拦截自述，2026-11-01](https://x.com/i/status/2116889254995570870)
- [补充：Gagan对可能的无障碍权限风险提醒，2026-11-01](https://x.com/i/status/2116910669853606170)
- [补充：作者答复将研究安全建议，2026-11-01](https://x.com/i/status/2116911120628019653)

[English](en/sujal-instagram-claude-reels-bounce-blocker.md) | [返回目录](../README.zh-CN.md)
