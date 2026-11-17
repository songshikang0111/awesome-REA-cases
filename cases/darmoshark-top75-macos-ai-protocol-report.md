# Darmoshark TOP75接Mac：AI辅助研究Windows工具，再以IOKit验证蓝牙命令

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-18
阶段：待验证

2026年11月18日01:24:07（北京时间），Bedirhan Skywalker（@bedirhansamsa）回答Darmoshark TOP75键盘的蓝牙协议从何而来：自己借AI逆向Windows配置工具，再用IOKit向已配对键盘测试命令。他说蓝牙复用USB的64字节命令，增加06 55前缀。补读同作者00:10:33主帖，目标是在macOS 14及以后控制RGB、改键、编辑宏和定时熄灯；主帖虽同在窗口内，但只是补充来源，不另算候选。未给模型名称或REA使用证据。

补充读取kreativecenter/top75-macos固定93650a4文档，提交2026-11-17 18:42:08 UTC，即11月18日02:42:08北京时间；这是候选后的文档快照，不能倒写成01:24时全部功能已实现。README把项目归于Bedirhan Samsa并链接同一X账号，说明为MIT社区项目。protocol.md记录静态检查Windows安装包与yc500_top75_soc、ID 957，交叉参考已有sharkfin协议文档，不是AI独立发现所有字段。蓝牙文档写66字节输出包承载前缀与64字节命令，读取响应并确认设备身份。

项目报告firmware 274上灯光、配置、短宏与选择性恢复的读回及回退，蓝牙定时熄灯后恢复旧设置。也记录五页宏写入曾导致USB重枚举，后改为按有效页写并限长；逐键颜色短间隔会丢写，现增加等待。显示图像通过USB，传输确认不是图像读回；静态图片经设备主人确认，GIF机上播放仍待验证。README称Apple Silicon实机测过，通用包支持Intel不是Intel实测证明；不把某台固件验证外推全系列。

本合集只读作者串、固定README与协议验证说明，未审完整源码或运行测试、安装Mac应用或连接键盘。文档中的验证仍是项目自报，不是独立复现；保留未核验状态。

2026-11-18候选封存0赞、11浏览、0转发、1回复；低传播不否定具体工程证据。验证是项目报告，非本合集测试。

## 来源

- [Bedirhan说明AI辅助Windows工具研究与IOKit测试，2026-11-18 01:24:07北京时间](https://x.com/i/status/2122742591888175234)
- [补充同窗口主帖：TOP75 Mac应用用途，2026-11-18 00:10:33北京时间](https://x.com/i/status/2122724078431748229)
- [候选后固定README：归属、能力与兼容限制，提交2026-11-17 18:42:08 UTC](https://github.com/kreativecenter/top75-macos/blob/93650a4f3e094cc5472a7eff18c1311dbbf5501c/README.md)
- [同一固定提交的协议与项目实机验证说明](https://github.com/kreativecenter/top75-macos/blob/93650a4f3e094cc5472a7eff18c1311dbbf5501c/docs/protocol.md)

[English](en/darmoshark-top75-macos-ai-protocol-report.md) | [返回目录](../README.zh-CN.md)
