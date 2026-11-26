# FreeCAD二进制到MCP：DeepSeek／REA研究原生接口的五任务对照

分类：应用与客户端 · REA
记录日期：2026-11-26
阶段：分析测试

2026年11月26日03:01:26（北京时间），Ao Qu（@ao_qu18465）介绍Agent-Native Computer Use：给Agent软件二进制和逆向工具，让它重接接口并构建MCP，不靠逐屏点击。03:33:26 morluto引用同一研究；本轮04:24:51，研究作者Paul Liang（@pliang279）明确与REA团队合作，再介绍FreeCAD演示55倍速度、35倍少Token。这些是同一研究的介绍，不是三次独立复现。

补充定位并阅读MIT-MI公开研究博客，固定提交c822a0c47cdea82fa28b3955a4216c80f1cc5db9时间为当日02:47:04，早于本窗口，属于补充文档而非新候选。博客明确输入FreeCAD 0.20.2二进制、REA、离线沙箱，无源码、文档、网络或评测任务。DeepSeek V4.1 Flash同时用于构建与任务；Agent从libpython3.11导出发现内嵌Python入口，以Frida注入脚本，在Qt主线程调用FreeCAD自己的Python API，构建85工具的服务。工具调用包含完整建模操作，而非一次鼠标点击；构建时尚未见评测任务，评测中不能改服务。公开代码库目录已定位，未逐文件审实现。

项目报告五项任务board-plate、cable-slot、service-standoffs、lid-vent、enclosure，分别9、10、10、13、21个输出文件检查，时限20、20、20、40、90分钟，各设置各跑三次。MCP通过全部检查，屏幕基线平均40%，初始文件本就能通过10%至33%，不是从零建模。五任务合计报告MCP 4.5分钟／3.1M Token，对照180.6分钟／127.1M，约各少40倍；调用数均值211对1466。演示lid-vent是44秒／0.64M对40分钟／22.2M，才是55倍／35倍口径，不是五任务总比值。

这些数值不含一次性服务构建；三次构建耗时37、30、85分钟。无REA消融仍能用窗口，却不能检查文件或进程，构建的服务未通过超出初始文件的检查。这说明本实验设定的差异，不是证明所有软件都要逆向或所有CAD任务都获相同提升。博客表格与方法是第一方报告，原始日志、完整评判代码、Token计费和统计不确定性未审，未重跑、构建、注入进程或安装依赖。Fruit Ninja为另一个既有游戏条目，不把它的成绩混作FreeCAD验证。

旧候选封存22赞、1227浏览、5转发、6回复；Paul Liang候选封存18赞、1160浏览、2转发、3回复。所有性能与检查数为研究方报告，未重跑。

## 来源

- [Ao Qu的Agent-Native Computer Use与FreeCAD比较自报，2026-11-26 03:01:26北京时间](https://x.com/i/status/2125666188630073806)
- [补充：morluto引用同一Agent原生接口研究，2026-11-26 03:33:26北京时间，非独立测试](https://x.com/i/status/2125674241169539568)
- [Paul Liang介绍REA合作与FreeCAD演示，2026-11-26 04:24:51北京时间](https://x.com/i/status/2125687177313198563)
- [补充固定研究博客：方法、五任务、消融与构建成本，提交2026-11-26 02:47:04北京时间，窗前文档](https://github.com/MIT-MI/Agent-Native-Computer-Use/blob/c822a0c47cdea82fa28b3955a4216c80f1cc5db9/index.html)
- [补充固定代码仓库目录，提交2026-11-26 02:06:11北京时间，未逐文件审实现](https://github.com/MIT-MI/Agent-Native-Computer-Use-Code/tree/eda0ba7fd7163deb09ee36f7e0c337af9bae5418)

[English](en/aoqu-agent-native-freecad-binary-mcp-computer-use.md) | [返回目录](../README.zh-CN.md)
