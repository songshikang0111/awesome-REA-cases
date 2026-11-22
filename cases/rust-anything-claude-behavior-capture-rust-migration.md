# rust-anything：先记录旧程序答案，再让Claude Code逐块重建Rust热点

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-22
阶段：待验证

2026年11月18日08:21:03（北京时间），codila（@0xCodila）介绍rust-anything：先运行旧程序记录常规与边界输入的答案，再让Claude Code逐块迁移到Rust，保留旧API并检查行为。这是从可运行实现提取行为，不是从闭源二进制恢复源码。08:31:36回复当时称检查文件写入、尚不支持网络与数据库；是早期边界，不应视作所有后来版本的现状。

11月18日14:14:25转述称Node.js搜索10ms到0.5ms、Python slugify17倍、Ruby shellescape11.8倍、浏览器WASM11.5倍及3万余用例零mismatch；17:57:32另一转述称搜索143ms到6.9ms、38251样本零不匹配，列TypeScript、Python、C、Go、Ruby、Java与Claude Code、Codex、Cursor、Gemini CLI、保留API及单设置回退。它们不是同次基准；最高20倍、免费、无需写Rust与Discord测试仍是推广说法。17:57帖封存43赞、1220浏览、3转发、17回复，其他历史快照在metadata，不把转述当独立测量。

11月20日10:42:45候选提v2.0.0／v2.1.0与Prettier17224次字节一致。当时补读固定提交a3f40af的README与real-world文档，原始提交11月20日07:08:15，早于当时严格08:00窗口，只作补充证据。工具不自动翻译，Agent或人写Rust，工具提供录制、桥接、diff与gate；MIT为项目声明。Prettier3.6.2示例按原格式器代码和输入输出重建打印器，用oxc解析，未支持构造则整文件回退原Prettier。旧文档报告17224／17224一致、15837次全在Rust、8.1%回退，不是纯Rust全覆盖。

11月22日15:42:40新候选细化v3.1.0、安装入口、语言阶段与录制风险。本轮读取发布元数据，确认v3.1.0发布时间为11月22日05:58:09，早于本轮12:00开始，只作补充。另固定提交783390fdc841ef42e8f1a7a805c1da1c2b56734c，原始提交11月22日15:51:01，在候选之后；README、STATUS与real-world为补充项目资料，不冒充候选帖当时已知的状态。

新固定README与real-world将Prettier修复后进度更新为17224次仍逐字节一致，其中15861次完整在Rust、7.9%回退，另有355个新增等价检查用例自报355／355；保留旧15837为历史里程碑，不混用为当前数量。十种格式语言不等于所有Prettier功能，HTML、若干配置、嵌入语言、解析边界和未知选项等仍会回退。STATUS区分六种已有真实项目逐单元运行的语言（TS／JS、Python、Go、Ruby、Java、C）、仅夹具测试的Kotlin，以及只能整应用analyze／record／replay／front-door、尚不能单元桥接的PHP与C#。其Kotlin Android夹具记录Android11 TV上291个录制用例、279／291匹配，12个未匹配尚未调查；不能把‘Tested’当完全通过。

项目原基准条件为Apple M4十核、16GB、macOS27.3、Node24.15.0、Rust release，两次运行、计时前比较输出。2360个JS／TS文件逐文件启动CLI为128.6／143.4秒对6.9／7.2秒，约19倍；预热进程内同集为4.2倍，不是通用19倍，也未因新用例自动重测。独立doc打印器跨桥反而变慢；早期文档还列gate只查port.rs、依赖crate须人工检查，以及app replay不带--build会重放原命令且不报回退率等限制，未在此证明后来全部消除。

新README确认setup为Claude Code、Codex、Cursor、Gemini CLI与OpenCode配置MCP及可支持的skill，先把已有配置备份为同目录的<file>.rust-anything.bak（可用--no-backup跳过）；有CLI、预编译、npm与插件入口。本条未安装或改动任何配置。record与app record会真运行原始代码，app record每例两次，diff／gate／replay也会重跑；文件、数据库和网络副作用会实际发生，须副本、测试数据库且无生产凭据。SMTP、webhook与SQLite副作用检查在STATUS仍是夹具Tested，不证明所有网络／数据库已等价。

以上为静态阅读的项目报告，未审完整实现、重跑用例、基准、回退或配置恢复；候选的7529星未核。匹配只覆盖记录输入，可读源码不等于唯一原始实现，REA未确认，状态仍unverified。

11月18日首帖封存31赞、1651浏览、3转发、10回复；最高20倍未核验，答案匹配仅限采集样本。
11月18日14:14:25介绍封存46赞、3270浏览、9转发、8回复；所称Node.js搜索20倍、slugify17倍、shellescape11.8倍、WASM11.5倍为不同热点。slugify是字符串转URL标识，shellescape是shell参数转义；该帖还列PHP/C#预览、录制、diff、bench、gate与回滚。本轮已补读仓库文档，原始样本、各语言完整覆盖、回滚与副作用等价仍未实测，旧宣传不等于新版本验收。
11月20日候选封存0赞、18浏览、0转发、0回复；帖子星数未核，不用热度证明17224次匹配。
11月22日15:42候选封存1赞、24浏览、0转发、0回复；7529星是转述，未核为当前热度。

## 来源

- [codila介绍rust-anything行为采集与Claude Code迁移，2026-11-18 08:21:03北京时间](https://x.com/i/status/2122847517725630555)
- [补充同作者回复：文件写入与网络/数据库边界，2026-11-18 08:31:36北京时间](https://x.com/i/status/2122850172455796799)
- [候选补证：语言支持、具名热点与性能数字的转述，2026-11-18 14:14:25北京时间](https://x.com/i/status/2122936447003136445)
- [新候选：143ms／6.9ms搜索演示、38251样本及API回退转述，2026-11-18 17:57:32北京时间](https://x.com/i/status/2122992595710472334)
- [Prettier迁移与17224次匹配转述，2026-11-20 10:42:45北京时间](https://x.com/i/status/2123607951864635839)
- [补充：固定11月20日07:08:15北京时间提交的README，早于候选窗口](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/README.md)
- [补充：同提交real-world文档，Prettier回退、基准与已知限制](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/docs/real-world.md)
- [v3.1.0、语言支持和录制风险转述，2026-11-22 15:42:40北京时间](https://x.com/i/status/2124408204746444826)
- [补充：v3.1.0发行，2026-11-22 05:58:09北京时间，早于窗口](https://github.com/erkamyaman/rust-anything/releases/tag/v3.1.0)
- [补充：固定11月22日15:51:01北京时间提交的README，晚于候选](https://github.com/erkamyaman/rust-anything/blob/783390fdc841ef42e8f1a7a805c1da1c2b56734c/README.md)
- [补充：同提交STATUS，真实项目与夹具、Android未匹配和副作用边界](https://github.com/erkamyaman/rust-anything/blob/783390fdc841ef42e8f1a7a805c1da1c2b56734c/docs/STATUS.md)
- [补充：同提交real-world，15861次纯Rust与7.9%回退及基准条件](https://github.com/erkamyaman/rust-anything/blob/783390fdc841ef42e8f1a7a805c1da1c2b56734c/docs/real-world.md)

[English](en/rust-anything-claude-behavior-capture-rust-migration.md) | [返回目录](../README.zh-CN.md)
