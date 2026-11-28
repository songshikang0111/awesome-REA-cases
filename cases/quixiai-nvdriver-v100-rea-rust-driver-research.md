# nvdriver：Eric Hartford用REA研究V100驱动，项目报告Rust重建与真机对照

分类：硬件与设备互通 · REA
记录日期：2026-11-28
阶段：进行中

2026年11月28日05:29:12（北京时间），Eric Hartford（@QuixiAI）介绍QuixiAI/nvdriver：想使用V100，却发现不能使用NVIDIA的开放驱动，于是为掌握驱动行为而逆向，明确感谢morluto的REA。他称已经修好，并把旧硬件限制归因于厂商推动升级；后者是作者对商业动机的判断，不是已核实的厂商意图，也不能把所有不支持都等同故意降速。

补读同日07:59:02的固定提交6543601569a1af4a9da65b84ec458ba65635caeb，其README称以NVIDIA 580.178.04的nv-kernel.o_binary为参考，重建no_std Rust内核核心及少量Linux C适配，目标是保持未修改CUDA用户态与原厂伴随模块的行为、寄存器和ABI兼容。文档报告82个Unicorn二进制oracle、2096项控制及6288个多状态用例，并称8张Tesla V100-SXM2-32GB真机在可丢弃VFIO虚拟机中对照原厂驱动，CUDA、PyTorch／NCCL和llama.cpp等测试无差异。这里oracle指把原二进制的执行行为作为比较基准，不是独立审计。

另读同提交的四卡PyTorch报告，文件标记passed、device_count为4、设备名为Tesla V100-SXM2-32GB，列PyTorch 2.5.1+cu124、cuDNN 9.1.0、NCCL 2.21.5、collective摘要与clean_unload=true；这是项目提交的记录，未核其执行环境或重跑原厂对照。支持矩阵把Maxwell、Pascal及Turing至Blackwell列为离线HAL／Unicorn检查，非Volta与连接显示器的真机仍需测试，Tegra不支持；README对离线检查数亦保留不同段落口径，不能从其中任一总数推导覆盖所有路径。保留进行中状态，不宣称所有GPU可用、全部功能等价或生产安全；未安装驱动、加载内核模块、下载目标二进制或执行仓库代码。

2026-11-28候选封存21赞、2403浏览、5转发、1回复；仓库验证数字为项目自报，不是本合集复现。

## 来源

- [Eric Hartford的V100／REA研究自述，2026-11-28 05:29:12北京时间](https://x.com/i/status/2126428149378388330)
- [补充固定README：支持矩阵、验证与限制；提交2026-11-28 07:59:02北京时间](https://github.com/QuixiAI/nvdriver/blob/6543601569a1af4a9da65b84ec458ba65635caeb/README.md)
- [同提交的四卡PyTorch／NCCL项目报告，未独立重跑](https://github.com/QuixiAI/nvdriver/blob/6543601569a1af4a9da65b84ec458ba65635caeb/reports/final-7cd1-pytorch-nccl-4gpu-rust.json)

[English](en/quixiai-nvdriver-v100-rea-rust-driver-research.md) | [返回目录](../README.zh-CN.md)
