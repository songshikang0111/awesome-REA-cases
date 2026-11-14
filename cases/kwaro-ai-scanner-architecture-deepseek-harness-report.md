# Kwaro AI扫描harness：Ibrahim称研究旧扫描器架构后用DeepSeek报告SQLi等发现

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-14
阶段：待验证

2026年11月14日20:31:22（北京时间），Ibrahim Auwal（@ibrahimatix0x01）称为学习架构，逆向了一个最大的前AI时代漏洞扫描器之一，并把这些材料与100多个安全工具、100多本Web／移动安全书、所称全部公开HackerOne报告交给自己的@kwaro_ai Agent。目标是让AI安全调查harness借鉴已有扫描系统的组织方式，不是宣称反编译完一款已具名商用产品。扫描器名称、版本及逆向方式均未披露。

作者报告首轮用DeepSeek花费不足30美元，得到一项SQL注入（SQLi）和20余项其他发现。没有目标范围、测试授权、原始输出、误报核查、漏洞确认或赏金回执；findings不能升级成20余个已确认漏洞。材料数量与全部公开报告的完整性也未核实。帖子没有明确AI是否直接承担扫描器逆向，能确认的是作者将架构研究与资料用于AI Agent，不能说DeepSeek独自拆出了旧扫描器。

年底前登上HackerOne排行榜是作者的未来预期，不是当前成果。REA未提及，没有源码、harness配置、复现实验或计费日志，本合集未执行扫描、读取漏洞目标或复验发现。按具体AI安全工具构建的作者报告收录，保留unverified及架构研究与扫描结果的证据分离。

候选封存62赞、1637浏览、0转发、0回复；低于30美元与发现数量均为作者自述，不是独立漏洞验收。

## 来源

- [Ibrahim Auwal的扫描器架构／Kwaro／DeepSeek首轮报告，2026-11-14 20:31:22北京时间](https://x.com/i/status/2121581756344058350)

[English](en/kwaro-ai-scanner-architecture-deepseek-harness-report.md) | [返回目录](../README.zh-CN.md)
