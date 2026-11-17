# Marvel vs. Capcom 2：Claude辅助反编译，公开文档区分代码匹配、ROM复用与移植

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-17
阶段：待验证

2026年11月16日01:02:06（北京时间），Pixel Cherry Ninja（@PixelCNinja）转述Marvel vs. Capcom 2用Claude反编译NAOMI街机与Dreamcast版本，并有PC／3DS移植。11月17日11:59:43，The Gaming Emporium（@McGroin83）补充开发者gibletto、v0.4街机测试菜单、Windows GPU渲染、CHD／GDI／CUE／BIN／ISO光盘输入与全机型3DS／2DS的60fps宣称。两条均为项目介绍，不是独立复现。

本轮定位gibletto/mvc2-naomi-dc，读取固定提交4ccf4b47496c015e4c629403b682905d9838800a的README与ports/README；该提交为11月16日20:41:11北京时间，早于本窗口，说明加入测试菜单与3DS图块缝隙修正。README明确披露Claude，称同一C／SH-4汇编树匹配出口与美国街机程序、Dreamcast主程序及354个角色覆盖文件；给出程序大小和SHA-1目标，声称街机18306例程／700文件、Dreamcast18991例程／773文件匹配。这里只读文档，没有运行比对或重新计算这些目标哈希，不宣布唯一原始源码恢复。

重要限制：字节匹配构建需要特定Hitachi SHC 5.1 Release 08及Sega SDK库；301个库模块中260个直接复用SDK对象，41个据项目反编译。街机还从用户ROM提取七个未使用模型、16 KB旧构建残留与8 KB Z80程序，所以整ROM相同不等于每字节都是恢复的源代码。README承认部分函数为匹配而使用不自然或不执行的语句。

移植文档说游戏代码直接编译到宿主，但缺少的库调用有桩函数，AICA声音仍模拟ARM7与DSP，3DS禁用DSP并可用简化混响；不把‘不是传统模拟器’理解成没有任何模拟。Windows以SDL_GPU走Direct3D 12或Vulkan，失败时回退软件渲染；文档给59.94fps游戏节奏，不是本合集实测性能。32位ARM Linux仅称可构建、尚未运行，x86 Linux还缺部分支持。3DS内存和CIA／3dsx有差异，不能凭宣传证明所有机型完整等价。

用户须自备原游戏资产；项目代码标AGPLv3，原作与SDK不随此获得授权。本轮查询v0.4标签API返回404，未进一步确认实际发布标签，不据此说项目不存在。未下载目标游戏、SDK、构建产物或依赖，未看视频、跑游戏、审完整源码／CI或测试矩阵。REA未提及，保持other-ai／unverified，公开文档是证据补强而不是复现。

11月16日封存88赞、2391浏览、11转发、7回复；保留原快照。
11月17日候选封存1赞、51浏览、0转发、0回复；100%和60fps仍为项目／转述主张，未独立测试。

## 来源

- [Pixel Cherry Ninja转述MVC2反编译、Claude与移植，2026-11-16 01:02:06北京时间](https://x.com/i/status/2122012277172052221)
- [The Gaming Emporium介绍gibletto、v0.4与PC／3DS功能，2026-11-17 11:59:43北京时间](https://x.com/i/status/2122540157496602800)
- [窗口前补充：固定README的Claude披露、匹配范围与ROM复用限制，2026-11-16提交](https://github.com/gibletto/mvc2-naomi-dc/blob/4ccf4b47496c015e4c629403b682905d9838800a/README.md)
- [窗口前补充：固定移植文档的渲染、桩函数、音频与平台边界](https://github.com/gibletto/mvc2-naomi-dc/blob/4ccf4b47496c015e4c629403b682905d9838800a/ports/README.md)

[English](en/mvc2-naomi-dreamcast-claude-decomp-port-report.md) | [返回目录](../README.zh-CN.md)
