# DuoDesk：Opus改造TwinDesk开源共享引擎，而非已证实逆向TeamViewer

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-01
阶段：待验证

2026年10月31日22:29:42（北京时间），Movez（@0xMovez）称用Claude Code／Opus5.5做出DuoDesk，让Windows PC和MacBook共享鼠标、键盘、剪贴板与跨屏文件，亦宣传旧笔电或平板副屏、免账户、无云与加密。标题声称逆向TeamViewer／AnyDesk，但步骤实际是交给AI一个当时未具名的开源屏幕共享引擎，读Windows、Mac、Linux、Android及原生输入辅助代码，再由11个并行Agent给约370文件换品牌，其中一个专管不要重命名的兼容字段。不能把现有开源代码改造说成从专有二进制恢复全部协议。

作者说搭GitHub Actions按tag产出.dmg、.exe、AppImage、.deb、.apk，Mac在云端Apple硬件编译；首次跨屏鼠标卡边，Opus读日志定位并补拒绝原因日志。另一次测试部署使在线站点下线，称20秒回滚并收走Agent部署权。两天、本人零行代码和恢复时间均为作者口径，没有工作流运行或日志证明。23:49:46同项目追加远端应用窗口、手机电话／短信／通知／摄像头桥接，以及Wi-Fi、USB、Bluetooth宣传，未逐项测试。

11月1日23:57:01，Ahmed Reza（@AhmedReza）回复Movez后续宣传，指出其仓库描述为TwinDesk的Aurora改版，第一步就是提供开源引擎，认为应注明原作者而非称逆向。补读0xCodez/DuoDesk固定提交50125ca0c4f73ab3253e739dd8a6ec9cf1a8444b的README，提交时间10月31日23:09:36北京时间，早于本候选窗口。Credits明确写是Inuka Asith的TwinDesk分支，采用GNU GPL v3.0并称保留原版权说明；也注明部分代码来自MIT许可DeskPad。仓库元数据的Aurora描述与评论对应，上游归属不再未知。

固定README是补充来源，不是新候选，也不证明所有重命名、许可履行或跨平台功能已被审计。保留已有来源与ID，纠正此前尚未取得明确上游的证据限制。未观看视频、检查安装包、审计代码或测试双机；加密／无云不是安全结论，站点回滚也不证明完整兼容。按AI辅助开源引擎适配的未核验报告保留，REA未提及。

较早首候选60赞、2553浏览、1转发；后续8赞、365浏览、0转发；新增质疑候选1赞、7浏览、0转发。
11 Agent、约370文件、两天、20秒均为作者报告，不是本合集计时或验证。
固定README确认自述分支归属，不等于许可证履行、加密或兼容性审计。

## 来源

- [Movez的DuoDesk／Opus步骤及失败修复报告，2026-10-31 22:29](https://x.com/i/status/2116538107017212194)
- [同项目后续手机桥接与连接方式宣传，2026-10-31 23:49](https://x.com/i/status/2116558255040180315)
- [Ahmed Reza指出TwinDesk改版与原作者归属，2026-11-01](https://x.com/i/status/2116922467797139641)
- [补充：DuoDesk固定README的Credits，2026-10-31提交，早于窗口](https://github.com/0xCodez/DuoDesk/blob/50125ca0c4f73ab3253e739dd8a6ec9cf1a8444b/README.md)

[English](en/duodesk-opus-open-engine-desktop-sharing-report.md) | [返回目录](../README.zh-CN.md)
