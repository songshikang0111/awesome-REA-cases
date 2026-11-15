# Coway Airmega IconS脱云：HTTP根证书、AI蓝牙研究与Web Bluetooth安装器的二手报告

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-15
阶段：待验证

2026年11月14日01:32:44（北京时间），一则帖子转述Coway IoCare空气净化器的脱云研究，背景是官方云故障、应用重写和账号封禁困扰。它称设备在设置时通过明文HTTP下载Amazon根CA，设备所有者用树莓派隔离网络、mitmproxy观察流量，再替换信任根让设备接受另一个MQTT端点，以便Home Assistant直接通信。MQTT是设备消息协议；这里是恢复用户自有设备的本地互通，不是本合集已发现的漏洞。

早帖另称蓝牙配网使用加密protobuf传Wi-Fi凭据与云配置，结合Android日志与反编译应用，AI约20分钟拼合协议。11月14日09:00:02的转述点名Coway Airmega IconS，称使用Android蓝牙调试日志和AI编码Agent，并发现配网载荷直接指定证书服务器URL。它还称已做出开源Chrome Web Bluetooth安装器，可将净化器直接配对本地Home Assistant，不需焊接或厂商云。

11月15日14:01:00的新候选将研究者称为Scott Goldman，并具体称AI通过adb采集Android蓝牙HCI日志、反编译官方APK，约20分钟还原加密算法，发现根证书和云API地址由手机在配网时发给硬件。HCI日志是主机与蓝牙控制器之间的记录；这里是转述的研究材料，不是本合集实际抓包。该帖继续声称Web Bluetooth脚本可改指本地Home Assistant并接Apple Home，无需拆机刷写或路由代理；零延迟是宣传措辞，没有测量数据。新增姓名与采集路径只是二手归属和方法细节，不是独立硬件验收。

没有取得原作者直达页面、源码仓库、固件版本、调试日志或安装器代码，开源与无需焊接均为转述；AI模型及具体Agent未明确。20分钟指蓝牙协议研究说法，不涵盖整个脱云工程。没有证据证明所有Coway型号或当前固件都适用，也未独立验收Home Assistant稳定性、安全性或完全离线运行。与已有Ryan Blass未具名净化器Agent群调查没有可核同一性，不强行合并。未访问凭据、下载目标、连接设备或执行配置，未确认REA，保持未核验二手报告。

11月14日早帖快照2赞、83浏览、0转发、2回复；20分钟为二手说法，无可复核日志。
11月14日09:00候选快照0赞、27浏览、0转发、1回复；不是安装器验证或型号兼容统计。
11月15日候选快照3赞、668浏览、0转发、2回复；零延迟未测量，不作为性能数字。

## 来源

- [Coway／IoCare脱云与AI蓝牙拼合转述，2026-11-14 01:32:44北京时间](https://x.com/i/status/2121295210550571018)
- [转述：Airmega IconS型号、证书URL与Web Bluetooth安装器，2026-11-14 09:00:02北京时间](https://x.com/i/status/2121407777146892459)
- [新转述：Scott Goldman署名归属与adb／HCI采集路径，2026-11-15 14:01:00北京时间](https://x.com/i/status/2121845904730890524)

[English](en/coway-iocare-ai-bluetooth-local-mqtt-secondary-report.md) | [返回目录](../README.zh-CN.md)
