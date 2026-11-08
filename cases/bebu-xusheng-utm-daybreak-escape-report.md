# UTM逃逸：bebu转述Xusheng的AI发现与开放模型利用链分工

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-08
阶段：待验证

2026年11月8日14:00:21（北京时间），bebu（@bebuu_ai）的候选同时转述Xusheng对UTM的完整guest-to-host逃逸链，称GPT-6 Sol与Daybreak Blue发现零日，再由开放模型写链。UTM是面向macOS和iOS的系统模拟器与虚拟机宿主；官方文档说明其基于QEMU，并区分QEMU与Apple设置。报道没有说明这次研究使用哪个后端、平台或UTM版本，不能据此指控所有后端都受影响。

原帖补取确认文字及图片附件存在，但未查看图片、取得原研究、利用日志、受影响组件、设备配置、CVE或厂商修复记录。所谓最新、完整链和模型分工都是bebu的转述，不是本合集复现；同帖另一目标VirtualBox的版本号不适用于UTM。Vals AI基准与费用数据也不是这条逃逸的证据。

补读UTM官方文档只确认产品和后端背景。该页面在11月9日取阅、未核原始发布日期，不能当作11月8日窗口内的漏洞验证。本合集未执行目标或利用、连接客体／宿主或安装依赖；REA未提及，不提供逃逸步骤。

共同候选封存3赞、389浏览、0转发；UTM与VirtualBox是两个目标，共用一个候选判断，不重复计帖子。

## 来源

- [候选：bebu转述UTM与VirtualBox两条链，2026-11-08 14:00:21北京时间](https://x.com/i/status/2119309027058590185)
- [补充背景：UTM官方文档的产品与后端说明，2026-11-09取阅，非漏洞验证](https://docs.getutm.app/)

[English](en/bebu-xusheng-utm-daybreak-escape-report.md) | [返回目录](../README.zh-CN.md)
