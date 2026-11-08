# Qwen3.8-27B-QSA：转述ryu15反推稀疏注意力以改善长上下文推理

分类：算法与功能重建 · 未确认使用 REA
记录日期：2026-11-07
阶段：待验证

2026年11月7日11:21:06（北京时间），FHILY（@Oluwaphilemon1）转述日本本地推理爱好者ryu15反推QSA（文中称Micro-Block Sparse Attention）的核心思路，适配到Qwen3.8-27B，并称Hugging Face已有名为Qwen3.8-27B-QSA的checkpoint。目标是降低长上下文注意力计算成本，不是恢复全部Qwen4架构；与Qwen4的关系仅为文中猜测。

转述称使用两张NVIDIA V100 32GB：128K上下文预填从约1598升至3114 tokens/s，64K从约2900升至4300以上；128K生成从20出头升至45以上tokens/s。文中说以学习到的索引组织四token微块，而非简单整体削减KV缓存，多数评测接近原稠密模型。这些都是发帖者转述的开发者指标，不是本合集测量；未取得模型地址、源码、原始评测集、运行配置、精度或质量分项，不能确认同条件比较或质量完全不变。

本条作为AI算法重建相关研究收录，未证明使用AI编程Agent协助逆向，亦未说明REA，rea保留unknown。没有核验产品命名、Qwen4尚未发布的断言或架构归属，不下载权重、不执行模型或目标代码，保持未验证。

候选封存1赞、297浏览、0转发；双V100、token速率和质量接近均为转述，未复跑。

## 来源

- [FHILY转述ryu15的QSA重建与吞吐指标，2026-11-07 11:21:06北京时间](https://x.com/i/status/2118906560877371747)

[English](en/ryu15-qwen-qsa-sparse-attention-reconstruction-report.md) | [返回目录](../README.zh-CN.md)
