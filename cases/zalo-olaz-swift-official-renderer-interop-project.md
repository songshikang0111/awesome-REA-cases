# Olaz原生Zalo客户端：SwiftUI承接官方renderer，Claude署名只证明可见补丁归因

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-14
阶段：相关项目

2026年11月14日14:26:40（北京时间），AI极客新闻（@aigeeknews）介绍逆向后用Swift重写的原生macOS Zalo客户端。Zalo是一款通信应用，此处目标是让用户用原生Mac界面访问其消息与通话，而不是发现服务器漏洞。候选没有说明模型、REA或逆向过程；补取原串也没有新增技术文字。

另行检索找到描述相符的公开qnguyen3/zalo-swift-re（Olaz）项目，阅读README与固定提交c81437e7614ec77e96a005c72bd00ecd4108074b下的逆向笔记。README明确并不重实现Zalo协议：它在WKWebView中无头运行官方app.asar的renderer，由Swift补齐Electron preload与主进程原本提供的接口，再以SwiftUI展示官方客户端状态。文档称450项preload桥表来自官方脚本，列出二维码登录、聊天、同步、通话等项目自报状态；创建群聊标为尚未实账号验证，不能把列表当全功能独立验收。

逆向笔记的来源是Zalo PC 26.10.20，记载分析日为2026年10月25日，包含早期demo引擎设想及后来SQLite宿主说明；不能用早期设计段落覆盖较新的README架构。2026年11月11日20:51:31 UTC（北京时间11月12日04:51:31）的公开提交修复WebSocket握手，说明旧调用失败导致收不到新消息，并带Co-authored-by: Claude Opus 5.5署名。这证明项目公开把该补丁部分归于Claude，不证明最初协议研究、全部450项接口或全客户端由AI发现。补充源码与提交早于候选窗口，仅作核对，不计新抓取候选。

README说首次运行从VNG获取官方运行时并检查签名，仍依赖官方代码，不是完全独立的Swift协议实现。文档注明非官方、可能与服务条款冲突，GPL-3.0与其中libsignal组件有关；不据仓库许可给官方运行时另授版权。候选短链目的地没有直接核对，项目匹配来自独立公开检索。这里只阅读文档与提交信息，未下载官方安装包、审查完整补丁、构建客户端、登录账号或验证消息安全；REA未确认，以有限AI参与证据的相关项目收录。

候选封存0赞、9浏览、0转发、0回复；共同署名不是AI工作量、质量或独立运行证明。

## 来源

- [AI极客新闻：Swift重写Zalo原生客户端，2026-11-14 14:26:40北京时间](https://x.com/i/status/2121489975040733330)
- [补充Olaz README：官方renderer宿主架构与功能限制，固定提交c81437e](https://github.com/qnguyen3/zalo-swift-re/blob/c81437e7614ec77e96a005c72bd00ecd4108074b/README.md)
- [补充逆向笔记：Zalo PC 26.10.20及宿主接口，文内分析日2026-10-25](https://github.com/qnguyen3/zalo-swift-re/blob/c81437e7614ec77e96a005c72bd00ecd4108074b/REVERSE-ENGINEERING-NOTES.md)
- [窗口前WebSocket修复提交与Claude共同署名，2026-11-12 04:51:31北京时间](https://github.com/qnguyen3/zalo-swift-re/commit/c81437e7614ec77e96a005c72bd00ecd4108074b)

[English](en/zalo-olaz-swift-official-renderer-interop-project.md) | [返回目录](../README.zh-CN.md)
