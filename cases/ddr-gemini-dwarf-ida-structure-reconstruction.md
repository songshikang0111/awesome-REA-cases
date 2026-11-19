# DanceDanceRevolution：Gemini整理DWARF结构，再用IDA补无符号版本

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-19
阶段：进行中

2026年11月19日16:23:28（北京时间），Dank 'n Derpy Gamer（@DankNDerpyGamer）描述AI辅助研究Konami的DanceDanceRevolution音游：把残留DWARF调试数据中的结构列表交给Gemini排序、列字节大小，再结合IDA反编译伪代码，补出不带DWARF的游戏版本中的数据结构。目标是跨版本补足类型布局，不是翻译游戏或恢复全部原始源码。

补读16:22:48同作者上文，确认DDR为目标；这条上文是补充语境，不另算候选。作者用can表述具体工作方法，未列游戏版本、结构名、字段偏移、ABI、模型版本、产物或回归测试。保留进行中的方法自述，不把DWARF排序等同正确推断无符号版本布局；未取得二进制、运行IDA或独立检查。未提REA。

## 来源

- [DDR的Gemini／DWARF／IDA工作方法，2026-11-19 16:23:28北京时间](https://x.com/i/status/2123331309422489899)
- [补充同作者上文：目标为Konami DDR，2026-11-19 16:22:48北京时间](https://x.com/i/status/2123331142162031028)

[English](en/ddr-gemini-dwarf-ida-structure-reconstruction.md) | [返回目录](../README.zh-CN.md)
