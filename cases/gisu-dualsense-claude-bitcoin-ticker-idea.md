# DualSense变BTC行情指示器：gisu分享Claude Code灯条与扳机提示方案

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-23
阶段：待验证

2026年11月23日05:47:11（北京时间），gisu（@0xGisu）称用Claude Code逆向自己的PS5 DualSense手柄，使灯条随Bitcoin涨跌变绿或红，跌幅越深R2越难按，并给读者一段约30分钟可做的提示。其具体方案是Windows上的Python应用，经USB调用现成pydualsense库，每10秒从免费CoinGecko API取BTC价格。提示要求以一分钟前价格决定灯色及变化幅度决定亮度，五分钟内变动超过0.5%时双马达震动一秒，24小时涨跌决定R2阻力，玩家LED按1%刻度显示24小时变化，按触摸板在终端输出价格与涨跌。

补取原帖确认作者与视频附件存在，但未观看视频、取得生成代码、运行手柄或核对API限制与各项效果。明确保留为硬件再利用的具体AI实现方案及作者报告；使用现成控制库不证明作者或Claude新解出了DualSense协议，提示里的所有要求也不自动是实测功能。30分钟不是可复核工时，帖子未提REA。本合集未安装依赖或访问行情API。

封存快照1赞、62浏览、0转发、1回复；视频附件未观看，30分钟为宣传口径。

## 来源

- [gisu的DualSense行情指示器自述及完整Claude Code提示，2026-11-23 05:47:11北京时间](https://x.com/i/status/2124620733267464627)

[English](en/gisu-dualsense-claude-bitcoin-ticker-idea.md) | [返回目录](../README.zh-CN.md)
