# ClaudeMom：本地兼容网关把第三方模型接入Claude Desktop登录式界面

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-19
阶段：相关项目

2026年11月19日15:02:00（北京时间），候选介绍BigPizzaV3/ClaudeMom：官方Claude Desktop的订阅登录与第三方API模式露出的功能不同，项目希望用户用自选Anthropic兼容上游，同时保留登录式桌面工作流。帖子描述本地网关处理账号与功能开关请求，不改客户端二进制；它是AI客户端行为兼容项目，不证明AI独立完成逆向。

补读公开仓库固定提交f8910fab4f83f3fcc5a817f9d08660577af7beaa的README；该v0.1.9提交为11月19日00:20:17北京时间，早于本窗口，只作项目文档补证。README确认核心crates/claude-local与Tauri＋React桌面端结构，称本地兼容服务应答账号和功能请求、对话转发至用户配置的Base URL与Key；还列cc-switch供应商导入、SenseVoice离线听写、Code页与命令行共用会话。

文档声称Chat／Code／Cowork、中文界面与电脑控制可用，但也指出较新macOS可能显示后台模式不支持，解除版本限制的选项默认关闭。因此不采纳候选所谓无条件满血、完全无风险或任意上游均兼容的推广结论。文档描述本机证书信任与请求接管，涉及信任和流量边界，不能仅凭只在本地就判断安全；未审实现、数据流、凭据处理、证书范围、签名公证或平台测试。本合集没有安装、改变证书信任或访问账号。README注明AGPL-3.0-only；未作法律或官方授权判断。保留related-project，REA使用与AI辅助研究步骤均未确认。

2026-11-19候选快照6赞、699浏览、0转发、2回复；阅读README不等于核验功能、隐私或桌面端安全。

## 来源

- [ClaudeMom本地桌面互通候选介绍，2026-11-19 15:02:00北京时间](https://x.com/i/status/2123310807639363714)
- [补充固定README：v0.1.9，提交2026-11-19 00:20:17北京时间，窗口前文档](https://github.com/BigPizzaV3/ClaudeMom/blob/f8910fab4f83f3fcc5a817f9d08660577af7beaa/README.md)

[English](en/claudemom-desktop-local-gateway-interoperability-project.md) | [返回目录](../README.zh-CN.md)
