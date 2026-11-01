# BLA对抗REA：公开诱饵与预算边界测试，不是不可逆向保证

分类：应用与客户端 · REA
记录日期：2026-11-01
阶段：分析测试

2026年10月29日15:45:00（北京时间），0xMarioNawfal（@RoundtableSpace）介绍BLA（Blind LLM Agents），称它向发布产物加入诱饵与预算消耗结构，在保持用户功能时让REA分析失败或超预算。补查npm元数据把bla-agents指向qybaihe/bla；这是防御自己软件的相关项目，不是重建某个第三方应用。

阅读仓库固定提交e5a566a3f544f69ef8bbe153e721f1555901578a的README及empirical-rea-validation报告。报告标注2026年10月27日09:56、Asia/Shanghai，Node v24.22.1、tshark 4.4.19，早于候选，只作补证。项目用样本加固前后对照调用真实REA分析路径，报告Go buildinfo超过1MiB、BEAM超过64块、ASAR头部超过16MiB，以及JavaScript语义预算、模型元数据嵌套、SQLite陷阱列与WASM表示预算等受限结果。

报告也保留反例和方法边界：EVM加固后仍status=ok，只接近4MiB输入上限；Flutter采用私有投影逻辑的复刻，状态仍ok；PTX文本未触发预算。ASAR错误说明可通过设置提高默认上限，不能把默认预算失败写成永久不可分析。Ghidra/Hopper、Frida、LLDB/GDB、Rizin、JADX等原生或动态路径未在该环境实测，固件与若干GPU格式被跳过。

README把14目标约612.5倍token、292.2倍成本明确列为内部估计，与实际分析器错误不同；14/14运行时等价是项目样本检查，不保证任意软件语义、性能或可维护性。文档v1.4.0是仓库阶段说明，查询到npm latest仍为1.1.0、发布于10月25日，不把它们当同一已发布版本。

这不是云LLM Agent端到端消耗预算、追逐诱饵或完整逆向失败的独立实验证明。固定报告也未给本合集可确认的REA精确修订。本合集未安装BLA、执行目标代码或重跑测试，只静态审读公开项目自述；按对抗REA的分析测试收录，保留公开代码与局限，不保证保护效果。

较早候选快照10赞、10035浏览、1转发；新增候选1赞、457浏览、0转发，不覆盖旧快照。
项目实测是受限样本的分析器路径；token/成本倍数为估计，未独立复跑。
较早补证：10月27日报告；固定仓库提交时间为2026-10-28T18:09:36Z，非本窗口新发布。
11月1日14:48:02的日语报道新增版本信息：GitHub 1.5.2向未签名APK添加外部方法调用的诱饵DEX，JADX实测仍为计划；1.5.1据称修复破坏Bun单体可执行文件的问题，npm仍报1.1.0。这是二手版本说明，未读取该版固定实现或重跑验证，不能把旧1.4.0材料当1.5.2的实测证明。

## 来源

- [0xMarioNawfal介绍BLA及对抗REA结果，2026-10-29](https://x.com/i/status/2115711483049083166)
- [补充：BLA固定提交README，区分实测路径、估计与未测能力](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/README.md)
- [补充：10月27日项目REA分析器加固前后验证报告，固定提交](https://github.com/qybaihe/bla/blob/e5a566a3f544f69ef8bbe153e721f1555901578a/docs/redteam/empirical-rea-validation.md)
- [补充：npm包元数据与10月25日发布记录](https://registry.npmjs.org/bla-agents)
- [新增：1.5.2 APK诱饵DEX与1.5.1 Bun修复的版本转述，2026-11-01](https://x.com/i/status/2116784310317732268)

[English](en/bla-counter-rea-budget-decoy-validation.md) | [返回目录](../README.zh-CN.md)
