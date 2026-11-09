# BLA对抗REA：公开诱饵与预算边界测试，不是不可逆向保证

分类：应用与客户端 · REA
记录日期：2026-11-10
阶段：分析测试

2026年10月29日15:45:00（北京时间），0xMarioNawfal（@RoundtableSpace）介绍BLA（Blind LLM Agents），称向发布产物加入诱饵与预算消耗结构，在保持用户功能时让REA分析失败或超预算。npm元数据把bla-agents指向qybaihe/bla；这是防御自己软件的项目，不是第三方应用重建。

旧补读固定提交e5a566a3f544f69ef8bbe153e721f1555901578a的README与empirical-rea-validation。报告标注10月27日09:56、Asia/Shanghai，Node v24.22.1、tshark 4.4.19；提交时间2026-10-28T18:09:36Z。样本调用真实REA路径，报告Go buildinfo超过1MiB、BEAM超过64块、ASAR头超过16MiB，以及JS语义预算、模型元数据嵌套、SQLite陷阱列与WASM表示预算限制。EVM仍ok且仅接近4MiB上限，Flutter用私有投影逻辑复刻仍ok，PTX未触发预算；ASAR上限可提高，不是永久不可分析。Ghidra/Hopper、Frida、LLDB/GDB、Rizin、JADX等原生／动态路径未实测，固件及部分GPU格式跳过。14目标约612.5倍token、292.2倍成本是内部估计，14/14运行时等价仅是样本检查，不保证任意语义、性能或维护性。

旧文档v1.4.0与当时npm latest（10月25日发布的1.1.0）不是同版。11月1日14:48:02日语转述GitHub 1.5.2为未签名APK添加外部方法调用诱饵DEX、JADX测试仍计划中，1.5.1修复Bun单体可执行破坏，仍报npm1.1.0；未读固定实现或复测。11月7日10:40:42，KitPloit（@KitPloit）介绍3.0.0保护二进制、ASAR、JS、WASM、Python与模型文件；署名已核。旧补查npm确认3.0.0于2026-11-06T09:16:07.184Z发布、仓库qybaihe/bla，读取时latest3.0.1。登记是窗口前背景，不证明新版效果；3.0.0代码／测试未审，旧固定报告不能验证新版所有格式。

11月10日01:55:31新候选援引i10x称，项目Electron样本从607 B涨至16.9 MiB，假凭据可能触发商店审查或安全扫描；建议加固后跑自己的测试、真实秘密留服务端。03:15:20另一候选说607字节变17MB后REA报错，九种格式类似，而截图驱动Agent可绕开此路径。两种大小单位和取整口径保留原样，不自行合成倍率；未取得i10x原文、新样本、Agent日志或截图路线实测，因此体积、九格式与截图限制均为转述，不是本合集新测量。它们补充了分发与审查代价、分析器和GUI路径的区别，而非证明所有Agent均被耗尽或所有截图Agent都成功。

这不是云LLM端到端追逐诱饵、耗尽预算或完整逆向失败的独立证明，旧报告REA精确修订亦未确认。本合集只读公开文本与元数据，未安装、执行目标或复测，保留分析测试，不保证保护效果。

较早候选10赞、10035浏览、1转发；11月1日1赞、457浏览、0转发，保留旧快照。
受限样本分析器路径；token／成本倍数为估计，未独立复跑。
10月27日报告不能验证3.0.0；11月7日候选2赞、663浏览、1转发。
11月10日两新增候选封存依次0赞／15浏览／0转发、0赞／7浏览／0转发；体积与截图路径未复测。

## 来源

- [0xMarioNawfal介绍BLA及对抗REA结果，2026-10-29](https://x.com/i/status/2115711483049083166)
- [补充：BLA固定提交README，区分实测路径、估计与未测能力](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [补充：10月27日项目REA分析器加固前后验证报告，固定提交](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [补充：npm发布登记，11月7日重读确认3.0.0日期与仓库](https://registry.npmjs.org/bla-agents)
- [1.5.2 APK诱饵DEX与1.5.1 Bun修复的版本转述，2026-11-01](https://x.com/i/status/2116784310317732268)
- [KitPloit的bla-agents-3.0.0介绍，2026-11-07 10:40:42北京时间](https://x.com/i/status/2118896395687981497)
- [新增：607 B至16.9 MiB与假凭据审查风险转述，2026-11-10 01:55:31北京时间](https://x.com/i/status/2119851392353345740)
- [新增：17MB报错与截图驱动Agent路径限制，2026-11-10 03:15:20北京时间](https://x.com/i/status/2119871480838148149)

[English](en/bla-counter-rea-budget-decoy-validation.md) | [返回目录](../README.zh-CN.md)
