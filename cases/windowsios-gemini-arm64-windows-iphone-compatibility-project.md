# WindowsiOS：Gemini辅助ARM64翻译与Windows兼容环境，项目称在iPhone上运行Windows11

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：待验证

2026年11月15日11:52:06（北京时间），Andrew111（@AndrewSignalZ）转述Ammaar Reshi使用Gemini4 Carbon，让Windows11 24H2在名为iPhone Duo的设备上运行。目标是在iOS应用内提供可交互的Windows ARM64环境，不是恢复Windows原始源码，也不是证明iPhone可裸机启动Windows。原帖说有演示视频，但本合集未取得或观看该视频。

补查定位ammaarreshi/WindowsiOS，阅读固定提交0071d6975287fd720b9046dfd3bd80b6f2aa765e的README；提交为2026年11月12日03:25:11 UTC，早于窗口，只作项目架构与归属补证。文档将整个bring-up归功于Gemini4 Carbon，同时明确建立在Henge／Husk的ARM64动态翻译与软件MMU、LinuxRunner、StikDebug、libslirp、EDK2及virtio-win等上游工作上，不能写成模型从零独立完成。

文档解释的兼容问题包括：在16KB Darwin宿主上支持Windows NT所需4KB页和进程ASID、修正独占原子指令及Prism非对齐内存访问，并提供UEFI／ACPI、NVMe、USB、音频与网络虚拟设备。项目称不用Hypervisor.framework，而是ARM64到ARM64的JIT与软件MMU；因此near-native是项目性能措辞，不等于无模拟、无虚拟硬件或已测得接近原机速度。Prism负责来宾中的x86／x64兼容，也不代表每个Windows应用都能正常运行。

README自称在iPhone19,4／A20 Pro／iOS27 TXM环境端到端验证，展示说明涵盖Edge、Antigravity2.31.0、音频、以太网及OAuth桥；还称有384MiB JIT、4.5GB来宾RAM与1.46GB空闲桌面内存。这些仍是项目自述，未检查截图真实性、测试日志、设备身份或性能数据。候选约12GB镜像也未核实，不把文档丰富程度当作独立验证。

构建说明要求Apple Silicon Mac与开发工具、合法取得的Windows ARM64映像及另备固件／驱动，使用LLDB辅助JIT；没有在此运行任何命令。README称代码为GPL-2.0-or-later，不分发Windows镜像，并列上游许可；未全审许可，不表示Windows或设备限制已获授权。按AI辅助系统行为适配与二进制翻译项目保留unverified，REA未提及。本合集未下载系统映像、安装依赖、编译、连接手机或复现。

封存候选1赞、33浏览、0转发、0回复；无独立性能或稳定性测试。
Windows11 24H2、Gemini4 Carbon、iPhone Duo及内存数值按来源原样归因，不将宣传中的native视为裸机运行。

## 来源

- [Andrew111转述WindowsiOS／Gemini与Windows11手机演示，2026-11-15 11:52:06北京时间](https://x.com/i/status/2121813465946022308)
- [窗口前固定WindowsiOS README：Gemini归属、上游、JIT／MMU架构与项目自报验证，提交2026-11-12 03:25:11 UTC](https://github.com/ammaarreshi/WindowsiOS/blob/0071d6975287fd720b9046dfd3bd80b6f2aa765e/README.md)

[English](en/windowsios-gemini-arm64-windows-iphone-compatibility-project.md) | [返回目录](../README.zh-CN.md)
