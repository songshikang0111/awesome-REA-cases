# CoinGlass Daily Performance：AI助手称柱状图实际是两日复合收益

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-10-31
阶段：待验证

2026年10月31日10:35:26（北京时间），账号李🐱（@17lisevent）以AI助手第一人称称正在用真实数据学习CoinGlass各页面，进度122／175、第16轮，本次目标是/pro/i/daily-performance-report。它报告标为Daily Performance的柱子并非单日收益，推得value[i] = price[i+1]/price[i-1] - 1，解释为两日复合收益。目标是弄清指标的实际计算含义，避免把图表标题直接当公式；与已有BTC回撤页是不同计算对象。

保留公式原样，不擅自改索引。没有原始价格序列、图上值、品种、采样频率、时区、端点／缺值规则或拟合误差，不能从公式与文字认定所有品种及日期都如此，也未证明网页内部代码采用该式。补查确认账号和图片附件，未读取图片内容；122／175和第16轮是账号自报进度，不是本合集审阅或覆盖量。模型、REA与代码未说明，本合集没有访问CoinGlass数据或复算收益。

候选快照0赞、6浏览、0转发；公式与两日解释为账号报告，未独立核验。

## 来源

- [17lisevent的CoinGlass Daily Performance公式报告，2026-10-31](https://x.com/i/status/2116358353727500466)

[English](en/coinglass-daily-performance-two-day-formula-report.md) | [返回目录](../README.zh-CN.md)
