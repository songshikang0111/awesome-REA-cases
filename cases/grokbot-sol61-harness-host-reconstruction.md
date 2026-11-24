# Grokbot：核心恢复、NewMax插件与Gemini／REA的不同作者报告

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-25
阶段：进行中

10月19日04:58（北京时间），@Stephen4171127（熊布朗）报告用三天逆向并跑通Grokbot的Agent Harness与Host核心执行链路，版本0.72.0-pre.11。新版外壳未研究，界面沿用旧版。原意是测试REA，但作者说明实际主要靠模型读代码、写分析脚本与对照验证，主力SOL6.1，不把成果全归于REA。远程环境据称是在其VPS上通过Docker部署Cursor universal的sand-box-latest镜像，路径为主Agent调模型、委派电脑子Agent、查看桌面截图、点击打开Chrome、子Agent回报。目的是恢复可运行、可修改的执行核心；可维护源码整理和剩余宿主能力尚待完成。补查确认作者，没有公开恢复源码、可复跑日志或独立验证，作者说仅自用、不准备传GitHub；三天与成功链路不证明整款功能等价。

2026年10月28日09:26:59（北京时间），Yangyi（@yangyi）另报告把Grokbot逆向为插件服务接到NewMax，从NewMax Mobile调度Grokbot云电脑，例如在云机上运行视频，称无需自己的Claude额度、许多操作不用另付API钱。补查原帖确认署名。按同一Grokbot目标追加不同作者的互通报告，不认定复用熊布朗代码、相同版本或部署。此帖未说明逆向是否用AI、模型、接口、认证、源码、成本结构或运行日志；AI是接入的服务对象，不能把此前SOL6.1归给Yangyi。费用与额度是个人使用主张，不等于服务永久免费、获准再分发或全功能恢复。

2026年11月25日01:04:42，Subham Surana（@TheSuranaverse）称让Gemini 4 Neon与Antigravity研究Grok Bot，并额外提供REA MCP，自称做到了。补取确认署名与图片附件，但未读图；没有版本、分析日志、代码、重建功能或运行对照，无法判断做到指何种成果。按同目标追加不同作者尝试，不借用熊布朗的执行链、三天或Yangyi的费用宣称，也不把Grok Bot模型本体视为已恢复。全条rea仍按原多作者记录归other-ai，最新报告明确提REA但未核调用。保持进行中，本合集未访问账户、云电脑或执行任何实现。

10月19日04:58候选快照6赞、523浏览、1转发、2回复；不是独立复现。
10月28日候选快照2赞、1527浏览、0转发；费用、额度与云电脑互通为Yangyi自述。
11月25日候选封存26赞、748浏览、2转发、2回复；未取得最新尝试的代码与对照。

## 来源

- [熊布朗的Grokbot核心恢复与SOL 6.1自述](https://x.com/i/status/2111924992384311338)
- [Yangyi的Grokbot到NewMax Mobile插件报告，2026-10-28](https://x.com/i/status/2115253966355431881)
- [Subham Surana的Gemini／Antigravity加REA MCP研究Grok Bot自述，2026-11-25 01:04:42北京时间](https://x.com/i/status/2125274422827495812)

[English](en/grokbot-sol61-harness-host-reconstruction.md) | [返回目录](../README.zh-CN.md)
