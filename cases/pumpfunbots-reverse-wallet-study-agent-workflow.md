# pumpfunbots-reverse：研究666个钱包后让Claude先读策略再配机器人

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-07
阶段：进行中

2026年11月7日06:19:53（北京时间），zostaff（@zostaff）介绍pumpfunbots-reverse：研究666个Pump.fun交易机器人钱包的链上行为，整理监控、首买、跟单、分析和曲线毕业等七种机器人模块，建议在改配置前让Claude Code阅读docs/strategy-research.md。这里AI参与有明确界限：帖子直接支持Agent阅读研究辅助使用，不证明666钱包调查本身由AI或REA完成。该项目不同于既有Pump.fun平台源码重建。

补读同作者公开仓库固定提交717ca4c38d02fd8d3d22843312a040fbe2d77960的README，提交为11月7日04:21:29北京时间，早于候选但在本窗，作为补充项目记录而非另一个候选。文档提供Node22+、三依赖、七模块、V3交易事件结构和研究文件入口，并把示例标为dry-run纸面交易。80%胜率、最佳五钱包与344钱包合计亏69 SOL来自帖子；README的策略分组口径另有89个Direct High-Freq钱包，未核对原样本和分组关系，不把这些数拼成统计结论。

没有读取钱包数据集、验证PnL、执行机器人、生成密钥、使用RPC或交易；不根据宣传中的keys never leave认定密钥处理已安全审计。文档有dry-run并不保证所有命令默认纸面运行。收益不代表未来结果，滑点、手续费、失败交易与选择偏差未核实；memecoin风险高。公开实现与使用方案可收录，但零猜测、免费及无需付费API不能覆盖Agent、RPC与链上成本。

候选封存22赞、918浏览、1转发；666、80%、69 SOL和纸面收益为作者／项目口径，非本合集测量。

## 来源

- [zostaff的666钱包与Claude使用流程，2026-11-07 06:19:53北京时间](https://x.com/i/status/2118830758810821103)
- [补充README：固定2026-11-07 04:21:29提交，项目自述非独立测试](https://github.com/zostaff/pumpfunbots-reverse/blob/717ca4c38d02fd8d3d22843312a040fbe2d77960/README.md)

[English](en/pumpfunbots-reverse-wallet-study-agent-workflow.md) | [返回目录](../README.zh-CN.md)
