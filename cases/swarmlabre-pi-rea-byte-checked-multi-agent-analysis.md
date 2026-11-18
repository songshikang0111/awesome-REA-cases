# SwarmLabRE：pi驱动REA，把多Agent发现与文件字节核对后再写报告

分类：应用与客户端 · REA
记录日期：2026-11-18
阶段：进行中

2026年11月18日19:40:50（北京时间），Nikolaos Chrysaidos（@virqdroid）说明SwarmLabRE的Agent运行在pi coding agent上，通过自己的会话层调用morluto的REA CLI。补读当日19:36:53至19:40:52作者串：项目针对AI恶意软件分析中无法分辨模型编造的问题，称支持ELF、PE和APK，最多六个Agent共享看板，发现先与文件自身字节核对，报告从检查过的事实构建，Agent散文另标为模型文本。

作者说样本只在宿主机解析、不执行，工具和Agent分置关闭网络的容器，模型密钥不进入两者。每次运行称以manifest.json封存输入输出SHA-256，swarmlabre replay离线重建报告，全部字节相同返回0、有差异返回1。

补充公开仓库检索定位virqdroid/swarmlabre，读取固定提交02db64afb5dce4060fbc06e36eed30a06e24d80a的完整README。该提交日期为11月15日20:06:04北京时间，早于候选，只作设计与验证边界背景。文档标alpha 0.1.0，在单台NVIDIA GB10、Linux arm64、Python3.12.3上构建检查；演示、测试和11个golden cases均用脚本mock，不代表真实模型质量。另报一次Qwen3.8 Flash Next对生成的良性ELF的六角色运行；列测试模型还有Qwen3.8 27B和CYBER-FROST 3.8，未取得原始轨迹。README明确无真实恶意软件检查，其他CPU架构未测，工具镜像当前仅arm64。

README把核对扩展为文件字节及本次工具日志，并明确byte-checked只证明偏移处有这些字节，不保证Agent解释正确；判定、家族和置信度仍属模型意见。离线录制可字节一致不等于第二次实时模型运行相同；manifest没有签名，改文件后重算哈希也可自洽。因此不能把回放当来源真实性、完整恶意行为识别或隔离安全证明。

串文与README均称MIT。已读署名、文字和文档，未审实现、安全文档全文、样本或测试日志，未看演示、安装依赖或运行目标。宿主解析风险、核对覆盖、密钥与模型通信路径未独立测试；保留进行中工具项目，不作安全认证。补读串文及旧提交只是候选补证，不作为额外候选。

候选封存0赞、19浏览、0转发、1回复；不是功能或安全验收。

## 来源

- [候选：作者说明pi／REA与会话层，2026-11-18 19:40:50北京时间](https://x.com/i/status/2123018588999049634)
- [补充作者串首：SwarmLabRE字节核对动机，2026-11-18 19:36:53北京时间](https://x.com/i/status/2123017595649396929)
- [补充：文件格式、六Agent与事实报告，2026-11-18 19:40:49北京时间](https://x.com/i/status/2123018587019358384)
- [补充：宿主解析、容器及密钥边界，2026-11-18 19:40:50北京时间](https://x.com/i/status/2123018592031797314)
- [补充：SHA-256封存与离线回放，2026-11-18 19:40:51北京时间](https://x.com/i/status/2123018595341123660)
- [补充旧提交README：alpha、mock与安全／回放限制，提交日期2026-11-15 20:06:04北京时间](https://github.com/virqdroid/swarmlabre/blob/02db64afb5dce4060fbc06e36eed30a06e24d80a/README.md)

[English](en/swarmlabre-pi-rea-byte-checked-multi-agent-analysis.md) | [返回目录](../README.zh-CN.md)
