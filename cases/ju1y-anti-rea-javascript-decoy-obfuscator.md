# Ju1y的anti-rea：JS局部改名与惰性诱饵，尚无对Agent有效性的基准

分类：应用与客户端 · REA
记录日期：2026-11-02
阶段：相关项目

2026年11月2日02:59:56（北京时间），Ju1y（@Jack_Ju1y）介绍anti-rea，称在构建期间或之后为JavaScript bundle改局部标识符并注入惰性诱饵，以干扰REA等AI逆向Agent。02:59:57同作者补充，灵感来自veritas对异常标识符干扰指纹脚本分析的调查。这是研究AI分析边界的防御相关项目，不是AI帮助逆向某个应用的成功案例。

补充GitHub检索找到同作者名JackJuly/anti-rea，阅读固定8577c6f886ef667582dca1dba10c3425f767e341的README，提交2026-11-01T18:48:23Z（北京时间11月2日02:48:23），早于候选；未直接验证短链映射。文档描述本地变量／参数改名、不可达分支中的文本，单文件、目录、Rollup输出、Vite6.4.5与Next16.4.3 App Router客户端集成，Next默认仅报告、改写需显式实验开关。

文档限定服务器和可识别第三方chunk跳过，混合Rollup／Vite chunk仅加惰性文本、Next跳过混合chunk；按文件名过滤不能可靠识别内嵌依赖。已命名构建文件不重算内容哈希，source map可揭示原代码，其他Vite版本与Next Pages Router未验证，针对REA／其他Agent的效果尚未benchmark。未执行源码、测试或安装依赖，保留为实验性机制而非不可逆向、运行等价或安全保证；不与其他同名ANTI-REA仓库混同。

主候选快照3赞、25浏览、0转发；灵感回复0赞、5浏览。
项目未benchmark对REA的实际效果；仅静态阅读，未验证运行等价。

## 来源

- [Ju1y的anti-rea实验项目发布，2026-11-02](https://x.com/i/status/2116968500334129501)
- [同串：指纹脚本研究的灵感归属，2026-11-02](https://x.com/i/status/2116968502414451121)
- [补充固定README：集成范围与未benchmark限制，2026-11-02 02:48北京时间](https://github.com/JackJuly/anti-rea/blob/8577c6f886ef667582dca1dba10c3425f767e341/README.md)

[English](en/ju1y-anti-rea-javascript-decoy-obfuscator.md) | [返回目录](../README.zh-CN.md)
