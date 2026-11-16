# CUDA++与Spark Secrets：Stapleton报告在GB10重建部分GPU用户态执行栈

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-16
阶段：待验证

2026年11月16日07:07:59（北京时间）的公开信介绍Michael Drake Stapleton的研究。信中将其工作描述为人类约束并指导Agent跨内核、语言、GPU栈和模型运行时开发，同时明确具体实现创意归属不确定。本条只整理GPU目标的技术自述，不评判信中对论文平台的法律指控、审稿或研究有效性。

信中引用‘Reverse Engineering the CUDA Software Stack’（Zenodo 23677465），称CUDA++是面向NVIDIA GB10的研究阶段GPU机器码工具链，可不使用NVIDIA专有用户态编译器、运行时、驱动库及数学库，但仍依赖NVIDIA开源Linux内核模块与签名固件。其报告的归档结果包括九个指定FP32操作的GPU／CPU序列穷举一致，以及1048576元素向量加法的代码和输出哈希与主机模拟器记录一致。信中另把2026年10月22日的全芯片1048576／1048576值测试列为背景，不当作本窗口新运行。

同一GB10目标的‘The Spark Secrets’（信中列Zenodo 24047504）进一步报告带屏障启动开销25.09至31.97微秒、115.14 TFLOPS、195.1 GB/s，以及35B模型四个提示中三个32／32 token ID一致、另一个31／32。信中明确这些是已达到的探针结果而非硬件极限，也不是完整CUDA生态的即插即用替代；单机测量和不完全token一致必须保留。

本合集读取的是公开信完整候选，不是论文或测试日志；补取两个相关Zenodo API遭403，未取得论文正文、归档代码、哈希清单或Agent轨迹。来源中的记录号仅供追溯，未核论文日期或内容。模型和REA使用未明确，AI参与只按信中人类指导Agent背景归因；未运行GPU工具链或验证性能，保持unverified。

封存候选1赞、71浏览、0转发、0回复；全部GPU数字为公开信转述的项目结果，未在本合集核算或复现。

## 来源

- [公开信中的CUDA++／GB10与Spark Secrets技术自述，2026-11-16 07:07:59北京时间](https://x.com/i/status/2122104354140205554)
- [信中所引CUDA栈研究记录23677465；正文未取得，API返回403](https://zenodo.org/records/23677465)

[English](en/stapleton-cudapp-gb10-user-stack-reconstruction-report.md) | [返回目录](../README.zh-CN.md)
