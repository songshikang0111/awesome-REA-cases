# Kaddo：REA辅助研究HeyClicky后公开Codex驱动的Mac助手

分类：应用与客户端 · REA
记录日期：2026-10-30
阶段：进行中

2026年10月30日14:23:15（北京时间），Katleho Nkoe（@kadd_nkoe）称用reverse-engineer-anything制作受HeyClicky启发、使用自己Codex订阅的Mac助手Kaddo，选择开源而非出售。公开检索补读KNkoe/Kaddo固定提交e2948ce44ed53bd5f042e5b71bc303bc0527a432的README，提交为当日07:12:26北京时间，早于窗口。文档确认观察并逆向已安装应用，是独立实验项目，功能和可靠性可不同，也不承诺维护周期。与基线另一作者Ayush Pratap的私人HeyClicky重建不是同一项目。

README描述原生macOS聊天、语音、屏幕上下文与后台Codex Agent；要求macOS14、Swift6与Xcode命令行工具、已登录且兼容的Codex CLI。后台Agent另需Apple Silicon、Python3.12、本地8765端口验证器、下载固定公开Laya模型与联网安装；没有验证器不运行。这里未审验证器实现或安全性，不把其存在当可靠行动认证。

语音音频发送到Codex realtime；主动建议可把本地识别屏幕文字与近期活动发送给Codex，聊天及附件走所选provider。工作区限制不等于完整文件隔离，屏幕、辅助功能、麦克风权限需用户操作授予；订阅也不保证无限额度，第三方服务另有条件。项目已移除复制的HeyClicky录音与第三方标志，事件声音当前静音。

自有代码声明MIT，依赖与模型有独立条款；文档列swift test，但live测试需登录且会真实操作。本合集没有安装、授权、下载模型、启服务或运行测试，未验证功能对等与隐私承诺，保留有公开实现的进行中项目。

候选快照0赞、17浏览、0转发；未以低热度排除具体项目。
固定提交2026-10-29T23:12:26Z；仅静态读README，未核验本地验证器与live测试。

## 来源

- [Katleho Nkoe的REA/Kaddo开源自述，2026-10-30](https://x.com/i/status/2116053300214665282)
- [窗口前固定README：实验状态、功能、验证器与隐私条件](https://github.com/KNkoe/Kaddo/blob/e2948ce44ed53bd5f042e5b71bc303bc0527a432/README.md)

[English](en/kaddo-rea-heyclicky-codex-macos-assistant.md) | [返回目录](../README.zh-CN.md)
