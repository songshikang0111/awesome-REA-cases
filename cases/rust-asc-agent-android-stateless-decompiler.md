# rust_ASC：供Agent按需查询APK与DEX的无状态反编译器

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-06
阶段：相关项目

2026年11月6日09:23:00（北京时间），Dopax（@tensorstaff）的开源清单推荐rust_ASC，称面向Agent和移动安全研究，适合DEX／APK分析，约125星。补充查找到描述吻合的MG1937/rust_ASC，阅读main所指0daddfb832b24bd0e43e76a9365eab4673db0cec提交的README；提交日期为10月28日15:13:22北京时间，早于本窗口，作为工具身份和接口上下文，不冒充本窗发布。

文档说明它是Python ASC的Rust实现，直接查询编译产物，不预建全局索引或磁盘缓存。可搜索字符串、类型、方法与字段引用，定位单类并反编译、列类／方法／字符串及解码AndroidManifest，支持多DEX；全APK伪代码导出复用radguard。MCP通过stdio暴露CLI查询，每次调用启动新CLI进程；extends／impl查询仅CLI支持，不能把两个入口当完全相同。用途是把可定位的安卓代码证据交给Agent，不是自动重建任意App。

项目以TelegramX、WhatsApp、Grab与TencentQQ给出字符串引用55／67／118／136毫秒，单类79／70／111／118毫秒，并以既有ASC套件的JADX数字对照；另一个383MB、41 DEX的QQ全量伪代码导出在32 worker下报告2.56秒。不同APK大小与单类、全量工作负载不能混算；文档的提速不证明输出语义完整、可重新编译或普遍胜过JADX。README标注Apache-2.0，许可正文未另查。本合集仅静态读文档，未下载APK、安装依赖、执行代码或复现基准；不推断工具由AI编写，也未确认REA参与。

候选整条清单封存0赞、15浏览、0转发；125星为清单口径，不是独立复核或正确率。

## 来源

- [Dopax开源清单中的rust_ASC，2026-11-06 09:23北京时间](https://x.com/i/status/2118514451947409450)
- [补充固定README：2026-10-28提交，接口及项目基准](https://github.com/MG1937/rust_ASC/blob/0daddfb832b24bd0e43e76a9365eab4673db0cec/README.md)

[English](en/rust-asc-agent-android-stateless-decompiler.md) | [返回目录](../README.zh-CN.md)
