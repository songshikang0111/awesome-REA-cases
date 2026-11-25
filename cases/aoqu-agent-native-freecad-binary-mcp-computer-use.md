# FreeCAD不用看屏操作：Ao Qu报告Agent逆向后二进制接MCP

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-26
阶段：分析测试

2026年11月26日03:01:26（北京时间），Ao Qu（@ao_qu18465）介绍Agent-Native Computer Use思路：不让Agent模仿人看屏操作，而是给编译后的软件与逆向工具，研究其实现，改造成适合Agent调用的接口，再构建MCP服务。其具体应用目标之一为FreeCAD，作者报告55倍速度、35倍少Token，以说明重塑工具接口可以降低GUI操作开销。

补取确认作者与全文，公开卡片标题为Agent-Native Computer Use: When Agents Reshape the Environment for Their Own Use，域名mit-mi.github.io，卡片摘要明确输入编译二进制与逆向工具包。没有取得博客正文或确切源码地址，未查FreeCAD版本、AI模型、MCP工具、任务、基线、计时边界、Token计费或成功率，不能把相对数值外推为全部CAD任务、所有Agent或端到端含逆向成本的性能。窗口内morluto后帖经引用元数据确认指向同一研究，不是独立复现。未运行二进制、生成模型或安装依赖；REA没有明说，归other-ai。Fruit Ninja是同帖另一个游戏目标，单独记载，不把它的效果当FreeCAD验证。

封存22赞、1227浏览、5转发、6回复；55倍／35倍为作者比较，未取得原始测试。

## 来源

- [Ao Qu的Agent-Native Computer Use与FreeCAD比较自报，2026-11-26 03:01:26北京时间](https://x.com/i/status/2125666188630073806)
- [补充：morluto引用同一Agent原生接口研究，2026-11-26 03:33:26北京时间，非独立测试](https://x.com/i/status/2125674241169539568)

[English](en/aoqu-agent-native-freecad-binary-mcp-computer-use.md) | [返回目录](../README.zh-CN.md)
