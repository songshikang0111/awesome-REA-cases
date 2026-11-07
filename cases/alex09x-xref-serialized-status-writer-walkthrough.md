# XRef：从status字段追到候选写入函数，而不是看名字猜作者

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-07
阶段：相关项目

2026年11月7日07:25:12（北京时间），Alexander Panasenko（@alex09x_dev）以谁修改status字段为问题介绍XRef walkthrough：字段名称不能识别写入者，要从键找到候选函数，再核对机器指令。用途是给人工分析者和AI Agent一条可追溯的二进制研究路线，而不是让模型凭字段名推断业务语义。

补读alex09x/xref固定提交7e4ab744e1991a487729c5b4272a2c7e204b81db的README；提交时间为11月6日18:07，北京时间，早于本窗，仅作项目背景。公开Rust工具面向x86-64 ELF与带DWARF unwind的薄型小端x86-64 Mach-O，支持交叉引用、布局恢复、切片、伪C与序列化字段搜索，并有只读本地stdio MCP与JSON接口。文档明确xref field把键连接到偏移与指令见证，再排名可能写入的函数；候选不是源类型或具体对象处理者的证明。扫描有函数数、代码量、边与30秒预算，命中上限须看coverage。ARM64、PE、fat/universal与仅compact-unwind输入不支持，macOS ARM版安装包不等于可分析ARM64目标。

README另列114次针对剥离符号的XRef自身的记录运行，和旧版0.0.5在Ryzen9 9950X、Linux6.8、暖页缓存下的单次耗时；不是本合集重跑或通用性能保证。Linux x86-64实进程观察需权限，probe/watch/trace会向目标增加trap，不能把全部live路径叫无扰动只读。当前status示例未提供目标文件、具体writer地址或完整输出，本合集只读作者文字与固定README，未运行工具、附加进程或验证语义，不推断调用REA。

候选封存0赞、70浏览、0转发；114次运行与速度为项目记录，未独立复现。

## 来源

- [作者的status字段writer调查路线，2026-11-07 07:25:12北京时间](https://x.com/i/status/2118847197810925971)
- [补充README：固定2026-11-06 18:07提交，早于窗口](https://github.com/alex09x/xref/blob/7e4ab744e1991a487729c5b4272a2c7e204b81db/README.md)

[English](en/alex09x-xref-serialized-status-writer-walkthrough.md) | [返回目录](../README.zh-CN.md)
