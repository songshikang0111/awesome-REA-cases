# Kindle Oasis 3：Codex排查越狱卡点，作者实际打开微信读书书籍

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-02
阶段：待验证

2026年11月2日17:55:05（北京时间），monkey-king.sun（@sunyuhua0205）报告把Kindle接到Mac，希望使用微信读书。补取原帖完整尾部：设备为第10代Kindle Oasis 3、32GB、固件5.17.1；最终采用Nosebleed配合本地预置越狱安装脚本v2.5.0，KOReader 2026.07.1的kindlehf包，以及finlater/weread.koplugin v1.6.0。是AI协助既有社区越狱与阅读互通，不是Codex发现新漏洞或原创阅读器。

作者称原先防升级占位文件使空间仅约60MiB。Codex识别USB信息、核对向导并备份，初试SpiderCat电子书打不开，校验一致但有.bad_file缓存标记；清理重试后停在executing一小时。日志里uid=0 euid=0只表明曾提权，不证明后续安装完成。改用Nosebleed并预置约5MB主体脚本，保留原项目二进制与主体脚本，收集输出；随后设备自动重启、出现“You are jailbroken!”完成文件。作者明确首轮卡住原因未确定，不能说证实网络故障。

安装日志仍有一条系统补丁组件异常，但作者继续报告KOReader能启动、微信读书扫码登录并实际打开一本书。阅读器与插件1125个文件完成复制与内容校验，清理旧占位文件后约26.6GiB可用。Codex负责电脑端检查、下载、备份、脚本准备和日志；人负责Kindle点击、重启、Wi-Fi与手机授权，密钥无需交给Codex。

所有版本、空间、文件数和阅读结果来自作者，没有原始日志、持久稳定性或本合集独立复现；其他机型与固件需重新核对。REA未提及。未下载越狱载荷、执行脚本、访问账户或操作设备。

候选快照0赞、48浏览、0转发；补取完整原帖，未检查附图。
uid=0不等于安装完成；完成标记与实际开书是作者报告的不同验证阶段。
复用社区工具，不能归为AI原创漏洞；首次卡顿原因与补丁异常未被抹去。

## 来源

- [monkey-king.sun的Kindle／Codex完整排障与开书报告，2026-11-02](https://x.com/i/status/2117193771062554902)

[English](en/sunyuhua-kindle-oasis3-codex-weread-jailbreak.md) | [返回目录](../README.zh-CN.md)
