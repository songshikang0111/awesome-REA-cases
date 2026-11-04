# Voyager扩展本地重建：Grok Bot五角色静态审计后仍遇滚动故障

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-05
阶段：进行中

2026年11月5日00:19起（北京时间），Francesco Faenzi（@francescofaenzi）连串介绍以Grok Bot分析并本地重建Voyager Chrome扩展，目标是去除遥测、云同步与过宽权限，同时保留本地提示面板。作者称原扩展开源、版本2.2.1，未取得可确认仓库、许可证或原始载荷，不把其风险措辞当已证实恶意。

作者让五个peer-bot担任Team Lead、Analyst、Spec Writer、Rebuilder和Verifier，分别处理静态调查、规格、实现与检查。其报告Analyst在限定OAuth、Drive同步和DOM观察器的任务下输出REA-evidence.md，列26项风险；蓝图要求移除存储OAuth令牌、Google Drive后台同步、MAIN-world观察器与宽泛host权限，并分开研究、交接、实现和报告目录。这里REA也被展开为Reverse Engineering Agent角色家族，未确认实际调用morluto/rea，故归因为unknown，而非工具使用认证。

首轮称97.5%成功，云依赖剥离但T29文件夹排序UI缺失。随后的操作者测试发现本地面板不能滚动，作者归因flexbox／overflow继承；第二轮CSS修补后仍不能滚动。蓝图建议继续用JavaScript与CSS覆盖并最终导出PDF，但候选未提供第三轮实际结果、测试清单或最终交付，不把未来操作要求当成功。26项不是独立确认漏洞数，97.5%也没有分母和验收记录。未运行扩展、查看完整审计产物或验证无遥测；本地化不自动证明安全或法律意义的clean-room。

封存五帖依次为0赞／31浏览、0／4、0／2、0／3、0／10，均0转发；保留低传播快照，不用架构宣传代替运行证据。

## 来源

- [Faenzi的Voyager／Grok Bot串首，2026-11-05](https://x.com/i/status/2118015167586033749)
- [同串peer-bot架构](https://x.com/i/status/2118015193779511448)
- [首轮静态审计与97.5%自述](https://x.com/i/status/2118015254110363927)
- [第二轮滚动修补仍失败](https://x.com/i/status/2118015266131239248)
- [同串重建蓝图与移除目标](https://x.com/i/status/2118015290550407647)

[English](en/voyager-grokbot-rea-local-extension-rebuild.md) | [返回目录](../README.zh-CN.md)
