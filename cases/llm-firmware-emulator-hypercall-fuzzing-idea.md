# Vita3K里的固件研究：Farenain尝试用hypercall连接LLM分析与内部fuzz驱动

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-28
阶段：进行中

2026年11月22日22:50:25（北京时间），Farenain（@Farenain）解释正在尝试hypercall，让仿真器内部进程与外部进程通信：外部LLM可配反汇编器研究固件模块，内部driver负责fuzz，也就是以变化输入测试行为。目标是让模型的静态分析与受控执行配合，而不是仅凭反编译文本猜测。补读同日21:18:59的父帖，作者明确说为fuzzsociety_org启动了项目，在PS Vita仿真器Vita3K中实现类似QEMU的hypercall，用于注入进程、测试PS Vita内部库和模块函数。该较早父帖只作目标背景。

2026年11月28日05:30:41的新候选更新数据流：内部driver通过作者写作hype-rcall的接口向仿真器外部进程请求数据，外部进程由LLM管理；作者称LLM已经反汇编固件，对适合fuzz的函数有了判断。补读同窗口05:30:40的父帖，明确说使用ChatGPT推进，思路类似TriforceAFL，Vita3K内部driver能访问内部模块和hyper-call。新报告比此前架构设想更具体，但不能据此确认模型自主完成闭环测试。

没有精确ChatGPT模型、反汇编器、接口源码、输入样本、端到端执行日志、覆盖率、崩溃或漏洞记录。ChatGPT参与和反汇编进展是作者报告，不是已证明联通或自动发现漏洞；未审所附图片。保留原ID与既有来源并追加更新，本合集未运行仿真器、固件或fuzz代码，REA未提。

11月22日候选封存2赞、25浏览、1转发、1回复；不以互动确认项目已接通。
11月28日新候选封存0赞、84浏览、0转发、1回复；没有fuzz验收或漏洞报告。

## 来源

- [Farenain的LLM、hypercall与内部fuzz驱动说明，2026-11-22 22:50:25北京时间](https://x.com/i/status/2124515851365761316)
- [补充父帖：Vita3K与PS Vita内部库目标，2026-11-22 21:18:59北京时间](https://x.com/i/status/2124492842613530964)
- [新候选：外部LLM进程、固件反汇编与函数选择，2026-11-28 05:30:41北京时间](https://x.com/i/status/2126428522696855806)
- [补充同窗口父帖：ChatGPT、TriforceAFL与内部driver，2026-11-28 05:30:40北京时间](https://x.com/i/status/2126428517890195789)

[English](en/llm-firmware-emulator-hypercall-fuzzing-idea.md) | [返回目录](../README.zh-CN.md)
