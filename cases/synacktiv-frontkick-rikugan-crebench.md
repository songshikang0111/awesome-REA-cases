# Frontkick与Rikugan：旧密码任务的提示词混杂与Rikugan 2.0重写报告

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-27
阶段：分析测试

2026年10月18日00:17（北京时间），@MalwareBibleJP 介绍Synacktiv的Frontkick/Rikugan比较。此前补读Matthieu Breuil于10月13日发表的原文，用于核对实验而非冒充新发布。目标是从去符号密码二进制识别算法和密钥，重新实现解密并取得flag。作者从CREBench选AES-128-CBC与ChaCha20，在hardcode_plain、O0条件下，以Claude 5.5 Sonnet为每种工具各跑每题四次，设累计输入输出100万token预算；不是全套基准评测。

旧实验中的Rikugan通过预定义工具与参数校验操作；Frontkick直接在Binary Ninja的Python环境运行生成代码，无逐动作schema校验。后者将已安装库与已打开二进制信息放入初始提示，旧于最近四轮的内容截到500字符，满上下文时压缩历史，并在代码报错时检索由Opus 5.5生成、经项目验证的Python示例。文章同时指出频繁截断影响提示缓存，计划改进；文中没有提供Frontkick下载入口。

原文笼统称Frontkick约省一半token、得分近三倍。此前按公开八次表逐项计算，token总量比约0.634，平均得分为85.9375/100对31.25/100，不能写成三倍成功次数。Frontkick第一轮AES仍耗1,007,262 token、42轮、得分0；Rikugan八次中六次超过100万token，预算并非未越界的硬保证。Rikugan反复尝试未安装的pycryptodome，未利用现有cryptography；Frontkick因明确库列表而使用后者。Synacktiv因此不认定CodeAct内在优于ToolAgent，建议对齐库提示再比较。这里是作者公开实验与本合集此前对表格的计算，不是独立重跑，也不保证真实软件或其他模型同样表现。

2026年11月27日06:16:03（北京时间），Buzzer（@buzz3r_）宣布Rikugan 2.0，称插件完全以C++重写，采用omc／libomc后端，并说明OMP已用C重写；支持Binary Ninja与IDA。作者称可接已有Claude、ChatGPT、Gemini或Copilot订阅，也可用API密钥或本地推理。这是工具版本与接入路径的发布报告，快于以往没有量化基准；本合集只确认原帖、作者和视频附件存在，未读取短链文档／发行包、运行插件或验证登录接入。新帖没有重跑上述CREBench任务，不能把旧差距当新版成绩，也不能从重写推断旧提示词混杂已消除。

旧候选日期2026-10-18 00:17北京时间；原文日期2026-10-13，是补充核查材料。
两题、每工具每题四次；库提示不对等，未独立重跑，不外推完整CREBench。
此前按公开表计算token比约0.634、平均分85.9375对31.25；分数不是成功次数。
11月27日新候选封存1赞、108浏览、0转发、0回复；2.0性能和模型接入未测试，旧基准不代表新版。

## 来源

- [旧候选：吉川孝志的实验整理](https://x.com/i/status/2111491684156752278)
- [补充原文：Synacktiv 2026-10-13 实验与逐次结果](https://www.synacktiv.com/en/publications/ufc-666-frontkick-vs-rikugan)
- [Buzzer的Rikugan 2.0重写与模型接入发布报告，2026-11-27 06:16:03北京时间](https://x.com/i/status/2126077551688712681)

[English](en/synacktiv-frontkick-rikugan-crebench.md) | [返回目录](../README.zh-CN.md)
