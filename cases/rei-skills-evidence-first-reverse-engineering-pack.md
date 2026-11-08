# REI Reverse Engineer：从12项技能到Rust桌面与双MCP证据桥

分类：应用与客户端 · REA
记录日期：2026-11-07
阶段：进行中

2026年11月3日02:07（北京时间），Batuhan（@AtamanCossack）介绍REI Skills里的12项证据优先逆向技能，覆盖二进制、APK、固件／IoT、Electron、WASM与协议，声称全库895技能、21个AI目标。固定94a5c23e4e39b70994c0b32736978f5704b15c23的旧README区分指令技能与另装Python 3.10+工作台：14项stdio MCP工具、124项目录元数据、11个需明确授权的静态外部适配。PATH检测不保证版本或许可，PE／ELF／WASM解析有边界；当时实时Ghidra／IDA／JADX／Frida和morluto/rea适配仍列计划。旧文档链接的WASM差分演示未在本合集重跑，895技能不等于895次成功逆向。

11月7日23:29:42的新候选中，同作者介绍正在构建Rust＋Python/MCP的REI Reverse Engineer，强调二进制身份、字节证据与复现。按名称和同一维护者查得公开独立工作台仓库，阅读固定78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95的README及桌面验证文档；提交为11月7日23:20:32北京时间，在本窗口，验证文档自标日期11月2日，是补充的较早项目自测而非本轮发生的实验。保留旧ID与旧来源，补充同一REI工作台的发展，不另增一条技能包。

新桌面是Craft Anything的MIT／Apache-2.0授权源码分叉，连接原Python工作台与单独固定的morluto/rea本地MCP；上游REA固定f72638f6b1f1a41851bf321472569c3265556961。项目报告Windows 11 x64、Rust 1.97.0、Python 3.14.7、Node 24.22.1环境构建并打开未签名0.3预览，发现14＋234＝248条外部路由。验证记录称通过桌面原生引擎，对同一八字节合成WASM调用Python识别／SHA256与上游REA字节熵，输出进入证据界面，未执行目标；两服务仍分别保存证据，不是合并数据库。完整schema初次超预算超时，文档改用紧凑发现schema，保留服务端校验。旧记录中REA适配仅计划的说法不再代表新桌面桥的当前状态；不由双桥测试推断其他实时分析器已实现。

固定README报告Rust AI/UI/CLI套件352测试，Python65项中64通过、一项可选工具跳过；较早桌面验证文档列127项桌面/UI测试，属于不同记录范围，不相加。12项技能通过结构校验，Experiential流式及模型列表为loopback集成测试，未做真实付费API或用户OAuth登录。全部248路由、反编译准确性、设备行为和AI重建质量未逐项验证，依赖仍有11项moderate告警。Python本体只做有界静态分析，不反编译或运行目标；证据bundle不包含原二进制，完整性哈希不证明结论正确。配置云模型可能把提示与工具结果发出本机。以上为项目文档报告，不是本合集独立复现；未安装依赖、启动MCP、构建桌面或读取凭据。

11月3日旧快照1赞、11浏览、0转发；11月7日候选1赞、10浏览、0转发。
124目录、14个Python工具、234个上游工具与248条路由为不同口径，不是248项功能验证。
352与127测试分别来自README和较早桌面记录；65项Python测试为64通过、一跳过，均为项目自报。

## 来源

- [Batuhan的REI REA技能包介绍，2026-11-03](https://x.com/i/status/2117317644756123796)
- [补充固定REI Skills README：早期能力状态与可选工作台，2026-11-03](https://github.com/rootcastleco/rei-skills/blob/94a5c23e4e39b70994c0b32736978f5704b15c23/README.md)
- [Batuhan介绍REI Reverse Engineer证据工作台，2026-11-07 23:29:42北京时间](https://x.com/i/status/2119089920086061235)
- [补充固定工作台README：桌面、双桥与验证边界，2026-11-07提交](https://github.com/rootcastleco/Rei-Reverse-engineer/blob/78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95/README.md)
- [补充桌面验证记录：自标2026-11-02，固定于11月7日提交，早于窗口的自测](https://github.com/rootcastleco/Rei-Reverse-engineer/blob/78fab825e6bbc4b1ae5accd63af1cfb9d4fc1d95/docs/DESKTOP-VERIFICATION.md)

[English](en/rei-skills-evidence-first-reverse-engineering-pack.md) | [返回目录](../README.zh-CN.md)
