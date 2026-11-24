# 实体iPhone给Agent测：Mike的Xcode、Appium与Frida三层研究流程

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-25
阶段：相关项目

2026年11月25日02:07:50（北京时间），Mike Takahashi（@TakSec）介绍自己给Agent做iOS应用测试的工具分工：Xcode加devicectl／CoreDevice经USB连接实体iPhone、安装启动和截图；Appium XCUITest加WebDriverAgent检查UI、点击输入、导航并在不同手机重复；Frida及其工具在越狱研究手机上hook运行App、追方法、读数据和提取解密后二进制。用途是跨设备／构建比较、运行时研究与发现只在iOS端出现的攻击面。

补取确认作者与图片附件，但未读图。没有App名称、iOS或工具版本、Agent模型、脚本、测试输出或漏洞披露，不能说已有自动发现或同等覆盖所有App。越狱研究机能力不能推广到普通未越狱设备；自动UI测试也不等于二进制语义恢复。未提REA或具体AI模型，rea标unknown，作为具体Agent研究流程保留；本合集未连接手机、运行hook或提取应用。

候选封存12赞、841浏览、0转发、5回复；工具清单不是具名漏洞验收或独立复现。

## 来源

- [Mike Takahashi的iOS Agent测试与运行时研究工具分工，2026-11-25 02:07:50北京时间](https://x.com/i/status/2125290307902423258)

[English](en/mike-takahashi-ios-agent-xcode-appium-frida-workflow.md) | [返回目录](../README.zh-CN.md)
