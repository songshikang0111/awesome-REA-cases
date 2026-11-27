# Forza Motorsport 4：AI辅助重编译，新增Apple Silicon预览与受限性能对照

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-27
阶段：进行中

2026年10月29日19:44:22（北京时间），The Gaming Emporium报道i2kiselev的Forza Motorsport 4静态重编译；当日09:13:11Z的固定0be771c6文档已承认AI辅助代码、脚本、文档及游戏二进制逆向，未指定模型或REA。11月27日11:23:19的新候选再次介绍0.3.2，强调实验Apple Silicon支持、音乐、音频与旧CPU改进、DLC修复和着色器准备。本轮补读160ef51f716ebc6f90692d368d68f3a820fcecfe的README、性能与macOS文档；该提交为11月15日14:47:30Z，属窗前补充材料，不是11月27日的新版本发布。固定正文已写0.3.3，不能把候选宣传版本当作当前唯一版本。

项目通过ShiftGlue把PowerPC代码预先转为C++，Windows编译到x86-64，Mac到ARM64，图形走Vulkan／Mac的MoltenVK。基于arcanite24的Pinyon Shift及ShiftGlue分支，致谢ReXGlue、Xenia与较早fm4-recomp，不把继承运行时和渲染器写成AI从零完成。FM4专用深度、相机及物体运动供DLSS／FSR2／3，新文档另列FSR4、Xbox360生涯导入和鼠标视角；键盘、图形菜单、Disc2、DLC及Project Forza Plus 4也有项目支持说明。

最高5120×2880和240fps上限不是同一测试。保留0.3.0的限定对照：Ryzen7 5700X3D、32GB DDR4-3600、RTX4070Ti SUPER16GB、Windows10 Pro22H2，Bernese Alps与11台AI车，每项约12秒、三次中位数，Console预设、升采样关。1x／2x／3x／4x平均233／232／156／102fps，相同机器固定Xenia Canary为102／88／68／45；5K为102fps，项目称2.3至2.6倍，不外推所有赛道、GPU或配置。170Hz显示器不等于渲染吞吐，Mac预览也不继承Windows性能数字。

旧文档仅支持PAL／USA1.0且报告Expert与约30场Event List；新固定文档报告四种Disc1（含Europe／USA Rev1即1.1）、World Tour至Professional、约70场Event List、Free Play、Test Drive、Autovista、照片、车库、回放与保存，并报告Xenia生涯导入及Project Forza Plus 4在1.0／Rev1盘测试。这是开发者扩展口径，不是本合集重跑；分屏、方向盘和多数AMD／Intel GPU仍未测，Xbox LIVE／Kinect不支持，Linux和方向盘仍在路线图。

Mac文档称M1以上、macOS14以上，贡献者在M1 Max和M3测试原版Free Play、60fps上限及一轮无错误Vulkan验证；外置NTFS加第三方驱动的安装到标题约9秒，但初次着色器会短暂掉帧。文档也保留DB9车顶几何和内存检查的规避方案、Clang21预编译头崩溃后禁用及尚未完整重测的边界；macOS14本身、Mac上的Project Forza Plus 4、比赛中FSR2／3画质仍待验证。构建回执不证明玩法验证或跨工具链字节一致。

用户须自备受支持的合法游戏盘并在本机生成，不分发游戏代码、资产或预编译游戏；Windows首装约十分钟是项目估计。上述均为开发者文档与二手报道，未独立测性能、安装、下载游戏、运行测试或重新编译。

旧候选封存1赞、81浏览、0转发；本轮封存0赞、81浏览、0转发、0回复。补查时热度不替换快照。
项目Windows单机短赛道三次中位数：5K102fps，不是5K240fps，也不是Mac性能；未独立复跑。
实验版，自备受支持Disc1；新文档含Rev1与Mac预览，分屏、方向盘、多数GPU及macOS14真机仍无全面验证。

## 来源

- [The Gaming Emporium报道FM4重编译与AI辅助，2026-10-29](https://x.com/i/status/2115771724390178926)
- [补充：FM4固定README，2026-10-29 09:13:11Z提交](https://github.com/i2kiselev/fm4-static-recomp/blob/0be771c68af81af5d74ca2e2c6284ec6b6642207/README.md)
- [补充：同提交的测试范围、环境和Xenia对照表](https://github.com/i2kiselev/fm4-static-recomp/blob/0be771c68af81af5d74ca2e2c6284ec6b6642207/guide/performance.md)
- [本轮候选介绍0.3.2与Mac预览，2026-11-27 11:23:19北京时间](https://x.com/i/status/2126154875775902054)
- [窗前补充固定README：0.3.3、AI披露与Rev1，提交2026-11-15 14:47:30Z](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/README.md)
- [同固定提交的性能条件与扩展离线测试范围](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/guide/performance.md)
- [同固定提交的Apple Silicon测试与未验证边界](https://github.com/i2kiselev/fm4-static-recomp/blob/160ef51f716ebc6f90692d368d68f3a820fcecfe/guide/macos.md)

[English](en/i2kiselev-forza4-ai-static-recompilation.md) | [返回目录](../README.zh-CN.md)
