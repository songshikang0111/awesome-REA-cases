# ASC：Dopax介绍给Agent按需读取APK的反编译器

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-30
阶段：待验证

2026年10月30日09:15:47（北京时间），Dopax（@tensorstaff）在开源盘点中介绍ASC，目标是让AI Agent分析Android APK时不必先全量反编译或建索引，而把包作为只读库按需抽取。作者称大包全局xref与单类反编译远快于JADX、内存占用低，并提到另有rust_ASC。它是具体逆向工具项目的二手介绍，不是某个APK分析成功的证明。

原帖署名已核对，但短链接所指仓库作者、版本、测试包、命令、计时与内存测量未独立取得；没有给快多少的可用分母。rust_ASC是否同作者/同实现不明，不把它另计独立成果。2.6k星是作者称来自10月30日GitHub API的快照，未经本合集核对，不能用星数证明性能。未安装、运行反编译器或分析APK；REA未提及，保留未验证。

共同候选快照0赞、37浏览、0转发；2.6k星与快于JADX均是作者口径，无独立基准。

## 来源

- [Dopax开源盘点中的ASC项目说明，2026-10-30](https://x.com/i/status/2115975920758538656)
- [候选所附ASC项目短链，目标未独立解析](https://t.co/c8SimeRxe3)

[English](en/asc-agent-android-decompiler-digest-report.md) | [返回目录](../README.zh-CN.md)
