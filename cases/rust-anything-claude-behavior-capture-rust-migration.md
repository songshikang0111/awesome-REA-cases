# rust-anything：先记录旧程序答案，再让Claude Code逐块重建Rust热点

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-20
阶段：待验证

2026年11月18日08:21:03（北京时间），codila（@0xCodila）介绍rust-anything：先运行旧程序记录常规与边界输入的答案，再让Claude Code逐块迁移到Rust，保留旧API并检查行为。这是从可运行实现提取行为，不是从闭源二进制恢复源码。08:31:36回复当时称检查文件写入、尚不支持网络与数据库；是早期边界，不应视作所有后来版本的现状。

11月18日14:14:25转述称Node.js搜索10ms到0.5ms、Python slugify17倍、Ruby shellescape11.8倍、浏览器WASM11.5倍及3万余用例零mismatch；17:57:32另一转述称搜索143ms到6.9ms、38251样本零不匹配，列TypeScript、Python、C、Go、Ruby、Java与Claude Code、Codex、Cursor、Gemini CLI、保留API及单设置回退。它们不是同次基准；最高20倍、免费、无需写Rust与Discord测试仍是推广说法。17:57帖封存43赞、1220浏览、3转发、17回复，其他历史快照在metadata，不把转述当独立测量。

11月20日10:42:45新候选提v2.0.0／v2.1.0与Prettier17224次字节一致。本轮补读erkamyaman/rust-anything固定提交a3f40af的README与real-world文档，原始提交时间11月20日07:08:15北京时间，早于严格08:00窗口，只作补充证据。文档明确工具不自动翻译，Agent或人写Rust，工具提供录制、桥接、diff与gate；MIT为项目声明，未安装或运行。

Prettier3.6.2示例按原格式器代码和输入输出重建打印器，用oxc解析，未支持构造则整文件回退原Prettier。项目报告17224／17224记录运行字节一致，其中15837次完整在Rust，回退率8.1%；不是17224个纯Rust用例或全语言替代。固定文档列十种语言，HTML和若干配置、嵌入语言及解析边界仍不覆盖；未知选项、被忽略文件等也可回退。

项目基准条件为Apple M4十核、16GB、macOS27.3、Node24.15.0、Rust release，两次运行、计时前比较输出。覆盖的2360个JS／TS文件逐文件启动CLI为128.6／143.4秒对6.9／7.2秒，约19倍；预热进程内同集为4.2倍，不能混成通用19倍。文档保留独立doc打印器跨桥反而变慢、配置问题修复、gate只检查port.rs而依赖crate需人工检查，以及app replay不带--build会重放原命令且不报回退率等限制。

新README还描述SMTP等副作用录制，不能由此声称所有网络／数据库已等价；录制仍会执行原代码并产生副作用，需隔离副本和测试数据。本合集静态阅读项目报告，没有审完整实现、重跑用例、基准或回退，没有核对帖子所称GitHub星数。记录匹配只覆盖记录输入，源码可读不等于唯一原始实现；REA未确认，保留unverified。

11月18日首帖封存31赞、1651浏览、3转发、10回复；最高20倍未核验，答案匹配仅限采集样本。
11月18日14:14:25介绍封存46赞、3270浏览、9转发、8回复；所称Node.js搜索20倍、slugify17倍、shellescape11.8倍、WASM11.5倍为不同热点。slugify是字符串转URL标识，shellescape是shell参数转义；该帖还列PHP/C#预览、录制、diff、bench、gate与回滚。本轮已补读仓库文档，原始样本、各语言完整覆盖、回滚与副作用等价仍未实测，旧宣传不等于新版本验收。
11月20日候选封存0赞、18浏览、0转发、0回复；帖子星数未核，不用热度证明17224次匹配。

## 来源

- [codila介绍rust-anything行为采集与Claude Code迁移，2026-11-18 08:21:03北京时间](https://x.com/i/status/2122847517725630555)
- [补充同作者回复：文件写入与网络/数据库边界，2026-11-18 08:31:36北京时间](https://x.com/i/status/2122850172455796799)
- [候选补证：语言支持、具名热点与性能数字的转述，2026-11-18 14:14:25北京时间](https://x.com/i/status/2122936447003136445)
- [新候选：143ms／6.9ms搜索演示、38251样本及API回退转述，2026-11-18 17:57:32北京时间](https://x.com/i/status/2122992595710472334)
- [Prettier迁移与17224次匹配转述，2026-11-20 10:42:45北京时间](https://x.com/i/status/2123607951864635839)
- [补充：固定11月20日07:08:15北京时间提交的README，早于候选窗口](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/README.md)
- [补充：同提交real-world文档，Prettier回退、基准与已知限制](https://github.com/erkamyaman/rust-anything/blob/a3f40af356abc13be3baf33bfe1ddf860440d1c1/docs/real-world.md)

[English](en/rust-anything-claude-behavior-capture-rust-migration.md) | [返回目录](../README.zh-CN.md)
