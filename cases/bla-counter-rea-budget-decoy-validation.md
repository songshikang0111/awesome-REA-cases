# BLA对抗REA：公开诱饵与预算边界测试，不是不可逆向保证

分类：应用与客户端 · REA
记录日期：2026-11-07
阶段：分析测试

2026年10月29日15:45:00（北京时间），0xMarioNawfal（@RoundtableSpace）介绍BLA（Blind LLM Agents），称向发布产物加入诱饵与预算消耗结构，在保持用户功能时让REA分析失败或超预算。npm元数据把bla-agents指向qybaihe/bla；这是防御自己软件的项目，不是第三方应用重建。

旧补读固定提交e5a566a3f544f69ef8bbe153e721f1555901578a的README与empirical-rea-validation。报告标注10月27日09:56、Asia/Shanghai，Node v24.22.1、tshark 4.4.19；固定提交时间2026-10-28T18:09:36Z，均为较早材料。样本加固前后调用真实REA路径，报告Go buildinfo超过1MiB、BEAM超过64块、ASAR头超过16MiB，以及JavaScript语义预算、模型元数据嵌套、SQLite陷阱列与WASM表示预算限制。

反例包括EVM仍status=ok、仅接近4MiB输入上限；Flutter使用私有投影逻辑复刻且仍ok；PTX未触发预算。ASAR可提高默认上限，不是永久不可分析。Ghidra/Hopper、Frida、LLDB/GDB、Rizin、JADX等原生或动态路径未在该环境实测，固件及部分GPU格式跳过。14目标约612.5倍token、292.2倍成本是内部估计，不是实付消耗；14/14运行时等价是样本检查，不能保证任意软件语义、性能与可维护性。

旧文档阶段为v1.4.0，当时npm latest为10月25日发布的1.1.0，两者不是同版。11月1日14:48:02日语转述称GitHub 1.5.2为未签名APK添加调用外部方法的诱饵DEX、JADX实测仍计划中，1.5.1修复Bun单体可执行文件破坏，当时仍报npm 1.1.0；未读这些版本的固定实现或复测，旧材料不是新版验证。

11月7日10:40:42，KitPloit（@KitPloit）介绍bla-agents-3.0.0，称以诱饵元数据、预算消耗与运行时等价保护二进制、Electron ASAR、JS、WASM、Python和模型文件。原帖补取确认署名。随后只读npm登记补证：3.0.0发布于2026-11-06T09:16:07.184Z、repository指向qybaihe/bla，读取时latest为3.0.1；登记日期早于本窗口，不是新候选，latest也不是保护效果证明。未审阅3.0.0代码、测试或完整变更，不能用旧固定报告证明新版所有格式有效。

这不是云LLM端到端耗尽预算、追逐诱饵或完整逆向失败的独立证明，旧报告的REA精确修订亦未确认。本合集只读公开文本与元数据，未安装、执行目标或复测，保留分析测试，不保证保护效果。

较早候选快照10赞、10035浏览、1转发；11月1日候选1赞、457浏览、0转发，不覆盖旧快照。
项目实测是受限样本的分析器路径；token/成本倍数为估计，未独立复跑。
10月27日报告与旧固定提交不能验证3.0.0；11月7日候选封存2赞、663浏览、1转发。

## 来源

- [0xMarioNawfal介绍BLA及对抗REA结果，2026-10-29](https://x.com/i/status/2115711483049083166)
- [补充：BLA固定提交README，区分实测路径、估计与未测能力](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [补充：10月27日项目REA分析器加固前后验证报告，固定提交](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [补充：npm发布登记，11月7日重读确认3.0.0日期与仓库](https://registry.npmjs.org/bla-agents)
- [1.5.2 APK诱饵DEX与1.5.1 Bun修复的版本转述，2026-11-01](https://x.com/i/status/2116784310317732268)
- [KitPloit的bla-agents-3.0.0介绍，2026-11-07 10:40:42北京时间](https://x.com/i/status/2118896395687981497)

[English](en/bla-counter-rea-budget-decoy-validation.md) | [返回目录](../README.zh-CN.md)
