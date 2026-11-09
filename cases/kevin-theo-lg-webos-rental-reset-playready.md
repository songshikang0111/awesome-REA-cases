# 出租屋LG电视：Kevin Theo用Claude做欢迎页与Pi重置，发现PlayReady残留登录

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-09
阶段：进行中

2026年11月9日17:17:25（北京时间），Kevin Theo（@kevintheo）报告度假出租屋三台LG电视在本机显示住客姓名、六种语言、Wi-Fi二维码、天气和本地建议。原厂不再更新该固件，他使用webOS Homebrew项目提供的root路径。每次入住结束由Raspberry Pi重置电视，作者称每台两至三分钟，退出Netflix、YouTube与Prime Video；Netflix删除应用数据后仍保持登录，直到隐藏的PlayReady存储也被清除。这个具体残留状态调查是案例的研究价值，不代表破解DRM或恢复其密码学。

作者明确每个版本由自己决策并在电视测试，Claude Code写代码，Codex、GLM、Muse、Grok审查。他说11月7日公共版得到38项发现，29项确认并修复，每项有先失败的测试；这些是作者的项目质检计数，不是29个独立核验漏洞。补取作者串，17:29:09回复称公开模板包含TV应用、Pi部分、测试和AGENTS.md，MIT许可、填入样例数据。仅确认回复措辞，没有取得准确仓库或读取源码与测试；此回复作补证不另计候选。

作者提醒root且不打补丁的电视必须置于住客不可达网络。未给LG型号、固件版本、完整重置范围或跨应用重新登录验证；两三分钟为自报，不能保证所有账户凭据已清除或电视安全。Homebrew的既有root能力不归为Claude新发现，REA未提及。本合集未连接设备、删除数据或执行项目。

候选封存1赞、135浏览、0转发；三台、六语、每台2—3分钟和38／29发现均为作者自报。

## 来源

- [Kevin Theo的三台LG电视欢迎页、重置与PlayReady排查，2026-11-09](https://x.com/i/status/2119721007988593136)
- [补充作者回复：公开模板、AGENTS.md与测试范围，2026-11-09 17:29:09北京时间](https://x.com/i/status/2119723960258465793)

[English](en/kevin-theo-lg-webos-rental-reset-playready.md) | [返回目录](../README.zh-CN.md)
