# 旧webOS遥测屏蔽受阻：T0mmy让Codex读固件、经SSH反复试探

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-28
阶段：进行中

2026年11月28日12:23:56（北京时间），T0mmy（@lightmare8）报告自己只帮忙输入SSH登录密码，其后由Codex从固件逆向推测规格，自行反复执行SSH命令、思考、回看固件。作者明确说已经陷入袋小路；这是可辨认的设备固件研究过程，不是自动修复成功。

补读窗口前11月26日22:56:26的同作者父帖，目标是旧webOS设备：作者称先以slopbro取得root、启动SSH、安装Homebrew，打算用Life's Good Without Spying屏蔽遥测，却发现OS太旧、似乎没有iptables，于是先做转储再考虑。这些前置操作是作者自述，不能全部归功Codex；缺iptables的判断也没有命令输出证实。

没有设备型号、webOS版本、固件hash、具体命令、分析日志或完成屏蔽的结果。未连接设备、运行目标或验证root与隐私效果，REA未提及。父帖只补背景，不作为本窗口另一个候选。

2026-11-28候选封存0赞、12浏览、0转发、0回复；未报告成功解除阻碍。

## 来源

- [窗口候选：T0mmy的Codex固件／SSH循环与停滞，2026-11-28 12:23:56北京时间](https://x.com/i/status/2126532519562797480)
- [窗口前父帖：webOS root、遥测屏蔽与缺iptables，2026-11-26 22:56:26北京时间](https://x.com/i/status/2125966919790682446)

[English](en/lightmare8-webos-codex-firmware-ssh-telemetry-attempt.md) | [返回目录](../README.zh-CN.md)
