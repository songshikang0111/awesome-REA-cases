# OpenWrt指定网关：Codex参考华硕交互，重做按设备配置入口

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-20
阶段：待验证

2026年11月20日21:36（北京时间），小京蛇（@xiaojingshe）嫌OpenWrt按设备指定网关要手工打标签与绑定，称让Codex参考华硕自定义网关设计，写了选设备、网关和DNS后保存的插件。具体重建的是交互工作流，不是声称反编译华硕固件或发现私有网络协议。

短链确认huladabang/luci-app-device-gateway；补读候选前11月20日12:37:02北京时间提交c593d0d4407dfa4505bf055afa01082ce1af682c的README。文档说明LuCI规则写入UCI，再由脚本管理dnsmasq DHCPv4标签、Option 3网关与Option 6 DNS，客户端需续租；插件不负责旁路由转发、防火墙或IPv6 RA。

项目只报告TP-Link TL-7DR7299、ImmortalWrt 24.10-SNAPSHOT加LuCI 24.10的r20功能验证；其他官方24.10可试、23.05／22.03待联测。官方25.12用apk，现有IPK不能直接安装；包未声明flock依赖。文档描述失败尝试恢复配置，但不当安全保证。本合集只读公开文档，未装包、运行脚本或连接路由器，不把单机报告泛化。REA未提及。

封存54赞、5254浏览、6转发、11回复；单机验证与兼容范围均为项目文档，未复跑。

## 来源

- [小京蛇的Codex指定网关插件介绍，2026-11-20 21:36北京时间](https://x.com/i/status/2123772350277812717)
- [补充：候选前2026-11-20 12:37:02北京时间固定README](https://github.com/huladabang/luci-app-device-gateway/blob/c593d0d4407dfa4505bf055afa01082ce1af682c/README.md)

[English](en/openwrt-codex-asus-gateway-workflow-rebuild.md) | [返回目录](../README.zh-CN.md)
