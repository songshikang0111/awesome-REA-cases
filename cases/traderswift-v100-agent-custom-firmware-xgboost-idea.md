# TraderSwift的三张V100：Jignesh Davda想让Agent改固件服务XGBoost研究

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-24
阶段：待验证

2026年11月24日13:17:29（北京时间），Jignesh Davda（@JigneshDavda）在TraderSwift AI长文中讨论模型链与算力成本。补读全文确认，他称现有代码由Claude Code驱动一至两个Codex实例，并尝试DeepSeek、Qwen；这只是既有编程背景，不证明这些模型已经逆向GPU。

文章后段提出具体遗留硬件idea：作者认为旧NVIDIA卡在不再被CUDA固件版本覆盖后会降价，XGBoost仍适合旧卡，因此想让Agent工作流改写自定义固件；他说已买三张V100作第一阶段试验，还在寻找容纳它们的服务器。XGBoost是树模型学习工具，目标是交易模型研究所需的低成本算力，不是已训练出获利模型。

原帖将CUDA与固件并称，未区分需要更改驱动、运行时还是卡上固件；本合集保留作者措辞，不认定V100已失去何种支持或固件重写确有必要。没有目标版本、二进制、兼容实现、固件权限、测试、吞吐或收益记录。三张卡是作者购置自述，不是已部署集群或性能证明。未访问交易数据、下载固件、执行目标或测试GPU；REA未提，保留未执行idea。

封存2赞、73浏览、0转发、1回复；三张V100是作者报告，未给固件或性能结果。

## 来源

- [Jignesh Davda的TraderSwift长文：V100、XGBoost与Agent自定义固件idea，2026-11-24 13:17:29北京时间](https://x.com/i/status/2125096443199524919)

[English](en/traderswift-v100-agent-custom-firmware-xgboost-idea.md) | [返回目录](../README.zh-CN.md)
