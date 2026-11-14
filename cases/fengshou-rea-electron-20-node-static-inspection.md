# Electron目录静态侦察：丰收称REA给出20节点、26关系，未保证运行

分类：应用与客户端 · REA
记录日期：2026-11-14
阶段：分析测试

2026年11月14日17:15:48（北京时间），丰收（@ai_fengshou）称没有安装Ghidra或登录账号，使用rea-agents的analyze-javascript-application命令及JSON输出检查一个Electron应用目录。Electron把网页界面放进桌面程序；此测试想在复刻功能前先看清主进程、预加载脚本与页面入口如何连接。目标应用未具名，不能据宣传补成某个商用客户端。

作者报告输出20个节点、26条关系：main.js创建窗口、preload.js挂在webPreferences上、index.html加载renderer.js；另报零IPC与零contextBridge暴露。IPC是进程间通信，contextBridge是Electron向页面暴露接口的一种机制。零值是该静态报告的计数，不证明程序没有动态通信、隐藏调用或安全问题。作者自己明确不保证运行时能跑，只把它当侦察。

补取原帖确认作者与文字，未读取附图、目录内容、JSON原始结果或测试答案表，也未运行REA。MIT与45.8万星是对工具的宣传，不是样本规模或正确率，不用作验证。与已有846字节IPC自测、隐藏网络调用样本分别保留：这里未证明同一输入，输出也不同。保留analysis-test及静态分析边界，不称其反编译完整应用或已经复制功能。

候选封存0赞、136浏览、0转发、4回复；20节点26关系是作者读出的工具输出，非本合集复测。

## 来源

- [丰收的Electron静态结构测试自述，2026-11-14 17:15:48北京时间](https://x.com/i/status/2121532538980311508)

[English](en/fengshou-rea-electron-20-node-static-inspection.md) | [返回目录](../README.zh-CN.md)
