# MousePods：Claude辅助RemoteHID研究，AirPods在Linux当鼠标与游戏头追

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-11
阶段：待验证

2026年11月5日21:17:00（北京时间）的中文复盘称，开发者让Claude Code帮助AirPods 3在Linux上做头控鼠标，约300次盲探失败后转向Wireshark、山寨耳机反编译和iOS框架伪代码。11月11日09:01:26，Darrel Ang（@darrelang）介绍项目名MousePods、AirPods 3／Pro 2和不改固件；09:22:59，Dopax（@tensorstaff）补充RemoteHID／AACP文档、无需苹果旁路设备与400余测试。两条新候选与旧目标合并，不当三次独立验证。

本轮终于定位公开starman-tech/mousepods，固定提交310c79b1751b6b590e5899e518d67026c76138d9，时间为11月10日23:53:15北京时间，早于本窗口；它是补充项目文档，不是本轮新发布。README署名Matteo Gaudioso，第一人称称与Claude作为结对工程师一起逆向：Claude做探测、跨项目静态研究、控制器与测试，人拿着耳机、决定方向并在硬件核对。约一下午是作者自述；本合集没有AI会话或独立硬件实验。

README及DISCOVERIES说明AirPods 3通过RTBuddy的RemoteHID虚拟HID路径，而Pro 2走SensorDataWX；接入AACP／L2CAP后算头部朝向，经uinput控制Wayland／X11指针，不需刷耳机固件。项目把AirPods 3和Pro 2列为实机验证，原发现环境为AirPods 3、固件营销版本6296592、Ubuntu 24.04、BlueZ 5.72、Python 3.12。文档称MTU 672看不到较大的传感器描述符、2582可见，但诚实保留Apple PnP DeviceID与重新配对在首次成功前同时变化，尚未隔离MTU单独是否足够；不能把其解释升级为已完成单变量因果试验。

项目测量由25Hz到最高约210Hz，并称约180Hz时23秒中有12次超过50ms空隙，因此推荐100Hz默认。这比旧转述约200Hz更具体，不能视作所有耳机稳定210Hz。充电盒内传感器关闭，主耳切换会取消流，静置时融合流可冻结。README列Bazzite上Pro 2的Assetto Corsa与ETS2头追，由贡献者henningnorden测试；Games页会在Proton前缀放TrackIR／FreeTrack DLL，故不是对主机和游戏完全无改动。指向校准只在模拟中测试，滑行、头颌手势与部分耳机仍实验；Windows／Android未支持，不能据“Linux”泛化所有发行版。

README现称400余测试，较早DISCOVERIES复现段仍写37项，两者是文档演进而非本合集计数或重跑。静态阅读test_mouse_off_by_default.py可见默认暂停、不动光标、暂停持久化及恢复既有游戏桥接的断言，不能据此宣称整个测试套件已通过或任意环境安全。代码标Apache-2.0、发现／文档／抓包标CC BY 4.0，要求归属；可选garmin-ble为AGPL-3.0-only，捆绑分发有额外义务。Garmin不是本轮候选目标，不另开案例。“首次公开”仍是项目在11月4日所查范围内的主张，未核历史优先权。REA未提及，本合集未安装依赖、运行工具、连蓝牙或改游戏，保持未独立验证状态。

11月5日封存11赞、1297浏览、0转发；保留为旧报道快照。
11月11日两候选封存依次0赞／25浏览／0转发、0赞／42浏览／0转发；358星是Dopax当日文字口径，不是本合集测量。
固定提交2026-11-10T15:53:15Z；项目报告实机、约210Hz和400余测试，未在本合集复现。

## 来源

- [旧中文复盘：Claude Code／RemoteHID／Linux MTU，2026-11-05](https://x.com/i/status/2118331749214175491)
- [Darrel Ang补充MousePods名称、Pro 2与不改固件，2026-11-11 09:01:26北京时间](https://x.com/i/status/2120320966144270592)
- [Dopax补充RemoteHID／AACP及400余测试，2026-11-11 09:22:59北京时间](https://x.com/i/status/2120326389081559054)
- [补充固定README：作者、Claude角色、支持与许可，提交2026-11-10](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/README.md)
- [补充固定DISCOVERIES：测量环境、MTU未隔离与掉流限制](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/docs/DISCOVERIES.md)
- [补充默认暂停与游戏桥接回归测试：仅静态阅读，未运行](https://github.com/starman-tech/mousepods/blob/310c79b1751b6b590e5899e518d67026c76138d9/tests/test_mouse_off_by_default.py)

[English](en/airpods3-claude-remotehid-linux-head-mouse-report.md) | [返回目录](../README.zh-CN.md)
