# 桌面应用免手点控制：Nathan称Claude用Ghidra／Frida研究并搭起harness

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-14
阶段：待验证

2026年11月14日05:53:25（北京时间），Nathan Broadbent（@ndbroadbent）称让Claude使用Ghidra和Frida逆向一款桌面应用，并自行搭建harness来控制整个应用，不再需要自己点击或键入。Ghidra用于程序静态研究，Frida常用于运行时观察和插桩；帖子明确点名两者，但没有列出本次各自恢复了哪些接口。harness在此指围绕目标程序搭建的控制层，不是重建其全部源码。

作者由此感叹现在可为任意应用做自定义MCP，但正文没有证明已交付通用MCP服务或覆盖所有应用。这是一款未具名应用的控制结果自述；缺少应用与版本、操作系统、模型细分、hook位置、工具输出、harness代码、操作清单和失败案例，无法核认所谓整个应用的覆盖率或速度。没有工时数字，不补写数分钟完成。补取原帖确认作者，不运行桌面目标或注入工具。REA未提及，状态保持unverified；同串另一作者的Empire Earth 2引擎是独立目标，另行记录。

候选快照5赞、337浏览、0转发、2回复；补查增长不覆盖封存快照，未见公开实现。

## 来源

- [Nathan Broadbent的Claude／Ghidra／Frida桌面控制报告，2026-11-14 05:53:25北京时间](https://x.com/i/status/2121360815257534508)

[English](en/nathan-broadbent-claude-ghidra-frida-desktop-harness.md) | [返回目录](../README.zh-CN.md)
