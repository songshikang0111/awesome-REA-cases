# Thumbwise：研究iOS主屏布局存储，再让Claude／Codex经MCP整理应用

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-28
阶段：相关项目

2026年11月28日06:18:04（北京时间），Drake（@Copypaster3000）向读者推荐Thumbwise，称因没有公开Apple接口，花数周研究iOS如何存储主屏布局，做出Mac上的Apple Configurator替代品。作者说Apply可写入所建布局并核对结果，包括空位、带设置的小组件和多页文件夹，同时有MCP让Agent读取使用数据。工时、接口缺失和精确写入都是作者报告，未逐项验证；不能据此声称AI完成了底层逆向。

11月28日补读公开网站确认产品名与AI互通路径：Claude或Codex通过MCP，在用户授权后利用布局和可用的应用使用数据排布图标，用户先预览，再选择Apply写入iPhone；网站称每次Apply前备份，可恢复旧布局。页面要求Apple silicon Mac、macOS 15以上、iOS 27 iPhone与USB数据线，不支持iPad或iPhone Duo。网站强调布局和活动数据保存在Mac，但接入外部AI后的数据处理并未由本合集审计，不能据营销文案保证隐私。

按逆向成果与AI控制互通的相关项目收录，不是独立复现的协议恢复案例。未取得布局协议、源码、读写日志或各类小组件的前后对照，未观看演示、下载客户端或连接手机；MCP与恢复功能只作项目所述能力，REA未提及。

2026-11-28候选快照1赞、41浏览、0转发、1回复；MCP用于操作逆向成果，未证AI参与原始逆向。

## 来源

- [Drake的iOS主屏逆向与Agent MCP自述，2026-11-28 06:18:04北京时间](https://x.com/i/status/2126440447379988902)
- [Thumbwise公开网站：授权、Apply、备份与环境要求；2026-11-28补读，无独立页面更新日期](https://thumbwise.app)

[English](en/thumbwise-ios-home-screen-reverse-mcp-agent-layout.md) | [返回目录](../README.zh-CN.md)
