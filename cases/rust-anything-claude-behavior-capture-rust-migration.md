# rust-anything：先记录旧程序答案，再让Claude Code逐块重建Rust热点

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-18
阶段：待验证

2026年11月18日08:21:03（北京时间），codila（@0xCodila）介绍rust-anything，目标是在不破坏旧应用行为的前提下，把慢的部分迁到Rust。帖子列Python、JavaScript、TypeScript、Go、Ruby、Java、C，描述先运行旧代码，记录常规和边界输入的输出作为答案基准，再让Claude Code分块重写、逐项对照。这是从可运行实现提取行为并重建，不是从闭源二进制恢复原始源码。作者建议真实输入、只迁热点、交付前比较速度，也可逐块迁整应用。08:31:36同作者回复称文件写入已检查，网络与数据库调用尚未支持；检查机制与结果未取得。

早帖最高20倍、免费、无需写Rust及Discord测试均为推广说法，未给原始实验；不能当Discord已验证工具。14:14:25后续转述给出Node.js搜索10ms到0.5ms、Python slugify 17倍、Ruby shellescape 11.8倍、浏览器WASM 11.5倍及3万余用例零mismatch，另称PHP／C#为预览。具体数字和历史传播快照保留在metadata；不同热点不代表整应用通用提速。

17:57:32新候选又称创作者演示中同一搜索由TypeScript的143ms到Rust的6.9ms，38251个记录样本重放零mismatch；它列TypeScript、Python、C、Go、Ruby、Java六种语言，Claude Code、Codex、Cursor、Gemini CLI，以及保留旧API、逐块选择和单设置回退。帖子同时含两个推广版本，不当两次独立实验；143／6.9与旧10／0.5是不同转述的数字，不能混为同次基准或据此计算普适提速。新候选封存43赞、1220浏览、3转发、17回复，日期为11月18日，不代表实现验收。

原帖及早串确认署名和流程，新帖只按二手演示叙述；未取得并审阅仓库、许可、代码、原始样本、硬件、计时与构建配置、账单或回退实测。零mismatch只约束记录输入，不能证明所有路径、副作用等价或早期网络／数据库限制已解决。未安装依赖、运行旧程序或执行迁移；REA只是另一个阅读主题，不证明本项目使用REA，保留unverified。

候选封存31赞、1651浏览、3转发、10回复；最高20倍未核验，答案匹配仅限采集样本。
11月18日14:14:25的后续介绍称Node.js搜索由10ms到0.5ms、20倍，Python slugify 17倍，Ruby shellescape 11.8倍，浏览器WASM 11.5倍，3万余用例零mismatch。还称支持Node.js/TS、Python、C、Go、Ruby、Java，PHP/C#为预览，并介绍录制、diff、bench、gate与回滚流程。slugify是字符串转URL标识，shellescape为shell参数转义；这些是不同热点，不是同一应用通用提速。没有取得仓库、原始样本、硬件、计时与构建配置、各语言覆盖或回滚实测；零mismatch仅约束所用样本，不证明网络/数据库副作用等价，也不覆盖早帖尚未支持的边界。候选封存46赞、3270浏览、9转发、8回复；本合集未安装或运行。

## 来源

- [codila介绍rust-anything行为采集与Claude Code迁移，2026-11-18 08:21:03北京时间](https://x.com/i/status/2122847517725630555)
- [补充同作者回复：文件写入与网络/数据库边界，2026-11-18 08:31:36北京时间](https://x.com/i/status/2122850172455796799)
- [候选补证：语言支持、具名热点与性能数字的转述，2026-11-18 14:14:25北京时间](https://x.com/i/status/2122936447003136445)
- [新候选：143ms／6.9ms搜索演示、38251样本及API回退转述，2026-11-18 17:57:32北京时间](https://x.com/i/status/2122992595710472334)

[English](en/rust-anything-claude-behavior-capture-rust-migration.md) | [返回目录](../README.zh-CN.md)
