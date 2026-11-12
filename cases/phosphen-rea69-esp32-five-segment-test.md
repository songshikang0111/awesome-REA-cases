# ESP32固件自测：Phosphen称REA6.9拆出五段并验证校验和与SHA-256

分类：硬件与设备互通 · REA
记录日期：2026-11-12
阶段：分析测试

2026年11月12日04:48:26（北京时间），Phosphen（@phosphenq）在REA6.9发布分支自测帖中，报告输入一个ESP32固件镜像，工具将其拆为五个segment，并验证checksum和SHA-256。这是具体固件容器解析与完整性检查报告，不是反编译出五个模块或重建出可刷写固件。

作者没有给设备型号、镜像来源、哈希值、段地址、参考解析器或验证输出；五段不等于五个分区，也不推断发现了漏洞或应用逻辑。帖子还列UF2、Intel HEX、Motorola S-record与U-Boot支持，但未报告这些格式的具体输入与结果，不将格式名单算作实测。

补取原帖确认正文与署名；视频、仓库提交和样本未审，6.9名称与构建来源仅为作者说法。与同帖自建应用暴露面自测是两个独立目标，来源共用但不重复计算整帖热度。本合集未下载镜像、执行REA、重算目标校验或刷机。

2026-11-12整帖快照29赞、755浏览、0转发；五段与校验通过为作者报告，未独立复算。
补读Espressif固定文档（10月1日提交，早于候选）：镜像含可变数量数据段，尾部checksum与可选SHA-256只检测损坏；simple hash不同于secure boot签名，不证明发布者身份、代码安全或REA本次测试通过。

## 来源

- [Phosphen的ESP32五段与完整性验证自述，2026-11-12 04:48:26北京时间](https://x.com/i/status/2120619685582401814)
- [补充Espressif镜像格式文档，2026-10-01 22:21:27北京时间提交；11月12日静态查阅，仅解释segment与完整性检查](https://github.com/espressif/esptool/blob/8aefcacb19cd100e23754d7a166d29015c4ba22c/docs/en/advanced-topics/firmware-image-format.rst)

[English](en/phosphen-rea69-esp32-five-segment-test.md) | [返回目录](../README.zh-CN.md)
