# OpenGlass Go：Kimi研究裸眼3D屏，Gemini收尾Armbian替代固件

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-22
阶段：进行中

2026年11月22日02:03:56（北京时间），Megabits（@Megabits_mzq）说自己移植了完整Armbian、写了解码补丁，还发现主线内核驱动bug，准备后续提交。补读同作者01:51:36及01:58:00原串，目标是Looking Glass Go裸眼3D屏，项目叫OpenGlass Go；作者认为其内部类似Orange Pi，使用H618、SD卡和控制显示及电源的STM32。作者将多数逆向与初期代码归功Kimi，最后收尾归功Gemini Neon，未量化节省时间；发现bug不等于已被上游接受。

补查公开Builder与Apps README及lkg-mcu说明：Builder当前提交5ca6710日期为11月22日01:04:25，Apps的df77557为11月21日21:56:58，均为原始提交日期，不是新候选。文档描述固定Armbian、Linux 6.18.63、U-Boot与Debian Trixie的ARM64镜像、DRM/KMS应用、3D图像视频预渲染、文件管理及Mac USB存储模式。lkg-mcu文档列串口读校准、通知Linux上线、关机和USB／独立模式切换，支持具体设备互通方向；未审核实现或协议轨迹。

项目自称AI辅助、真机测试与人工设计审查，Apps甚至标称100% AI编码；均是项目归因，不是贡献审计。构建文档明确静态镜像验证不替代设备测试；须保存原SD卡及数据，第三方固件可能损坏设备或失去保修，组合镜像组件各有许可。未下载镜像、执行构建或刷写设备，未验证所有媒体兼容、解码效果或驱动bug，状态保留in-progress。

候选封存0赞、76浏览、0转发、0回复；仅原候选计入判断，原串与仓库为补证。

## 来源

- [Megabits说明Kimi／Gemini分工、Armbian与解码补丁，2026-11-22 02:03:56北京时间](https://x.com/i/status/2124202164860150025)
- [补充：OpenGlass Go首版与Looking Glass Go背景，2026-11-22 01:51:36北京时间](https://x.com/i/status/2124199061767221414)
- [补充：H618、SD卡与STM32结构，2026-11-22 01:58北京时间](https://x.com/i/status/2124200670786134462)
- [Builder README，固定11月22日01:04:25提交，后续补读](https://github.com/megabitsenmzq/OpenGlass-Go-Builder/blob/5ca67100645fc09d6de8fa217067ec0f37124890/README.md)
- [Apps README，固定11月21日21:56:58提交，后续补读](https://github.com/megabitsenmzq/OpenGlass-Go-Apps/blob/df775577dd9f361c17c0bbcb3918e9598e4cef99/README.md)
- [同Apps提交的STM32串口工具说明](https://github.com/megabitsenmzq/OpenGlass-Go-Apps/blob/df775577dd9f361c17c0bbcb3918e9598e4cef99/lkg-mcu/README.md)

[English](en/openglass-go-kimi-gemini-armbian-firmware.md) | [返回目录](../README.zh-CN.md)
