# X6200不用切回原厂系统：Claude辅助重建Xiegu基板升级流程，OpenX6X00已合并

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-16
阶段：待验证

2026年11月16日02:37:52（北京时间），KF（@d0tslash）介绍Claude辅助的开源贡献，指向OpenX6X00 PR259。Xiegu X6200是收发信机，OpenX6X00是其第三方界面／系统项目；问题是更新负责DSP、射频、功率与电键的基板固件时，原流程需要切回Xiegu系统并换卡。目标不是破解固件签名，而是在第三方系统中重现原厂升级程序。

补读Guru-RF/OpenX6X00 PR259：创建于11月13日18:55:41 UTC，早于本窗口；11月15日18:25:42 UTC（北京时间11月16日02:25:42）已合并，取阅时closed。作者MAVProxyUser称反汇编Xiegu应用1.0.8的UPGRADE路径，跟踪工作线程、握手、传输及CRC，写出C writer、Python流式提取器、GUI与SSH路径；PR结尾标Generated with Claude Code。基板自己的bootloader解密原厂.xgf文件，不需获得密钥，也未在PR分发Xiegu固件。REA没有提及，不把全部逐函数发现自动归给Claude独立完成。

文档报告CRC对照2000个随机包、SHA／文件选择测试与模拟基板的成功和失败路径。补读head 9612ae8522ce1b57383614d44d588be0317cd1ad的check-runs，返回一个test任务completed／success，完成于11月15日04:59:02 UTC；这是项目CI记录，不是本合集重跑或实机认证。作者另报11月13日单台X6200在其fork中进行1.0.7→1.0.8、回退、再升级三次，传输分别32.4、27.9、32.4秒，校准保留；流式取文件在371MB zip读到255MB时完成，272秒、68MB内存，均未独立测量。

限制明确：不适用X6100，无法读回基板flash所以没有运行固件备份；擦除后恢复依据设计，尚未遇到实机失败而验证。作者测试用了11.8V并保留电池，不符合文档列出的原厂供电条件，不能当刷写建议。相邻gdyuldin/x6200_gui PR15在11月13日创建，迁移同一writer但明确没有在该GUI镜像实机跑过；它是补充背景，不是第二个独立项目或本轮新候选。

本合集只读PR、API状态与CI记录，未执行下载代码、目标测试、安装依赖、下载原厂固件或接设备；合并与CI成功不等于所有升级安全，硬件结果保持unverified。

候选封存1赞、101浏览、0转发、0回复；11月13日三次刷写是作者测试，不是三台设备。
合并状态和固定head一个成功check经API补核；单台供电、无flash读回及恢复未实测限制保留。

## 来源

- [KF介绍Claude辅助OpenX6X00 PR259，2026-11-16 02:37:52北京时间](https://x.com/i/status/2122036376723951618)
- [原PR259：创建2026-11-13，2026-11-16 02:25:42北京时间合并；原厂流程与作者单台测试](https://github.com/Guru-RF/OpenX6X00/pull/259)
- [固定head的项目test成功记录，完成2026-11-15 04:59:02 UTC；未在本合集重跑](https://github.com/Guru-RF/OpenX6X00/actions/runs/43678985278/job/132705273774)
- [窗口前关联PR15：同一writer迁移，2026-11-13创建；目标GUI镜像未实机测试](https://github.com/gdyuldin/x6200_gui/pull/15)

[English](en/x6200-claude-base-firmware-upgrade-reimplementation.md) | [返回目录](../README.zh-CN.md)
