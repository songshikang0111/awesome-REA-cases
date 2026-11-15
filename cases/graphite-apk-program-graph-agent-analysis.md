# Graphite：把APK调用链与数据流变成Agent可查的程序图，不需要源码

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：相关项目

2026年11月15日20:03:03（北京时间），Johnson Li（@jingsenli）回复称，即使只有APK，Agent仍可查询整个应用的调用链与数据流，了解值从哪里来、各部分如何连接。补读11月15日00:19:46的较早父回复，确认工具是johnsonlee/graphite，而不是本合集既有Apkscope；该父回复把Graphite称为REA的助力。父帖早于本窗口，只用于定位，不当新候选。

补读固定d4dd8ee618b0345bb91de3f90c7c238b3f4425f9 README，提交2026年11月14日13:53:37 UTC，早于窗口。Graphite将JVM字节码等输入建成程序图，以调用、类型与数据流关系提供上下文，让LLM经MCP发Cypher查询，也有CLI和Explorer。APK分析需Java及Android平台jar；文档的JVM无源码路径不等于Swift／Objective-C也能只靠任意二进制分析，Apple前端依赖编译索引与声明。

文档明确静态图覆盖取决于所包含类、依赖和支持模式，反射与动态加载会导致未解析关系。README的规模、延迟、CodeGraph对照和openCypher兼容数字未在本合集重跑，不能证明所有APK可完整恢复或所有查询正确。本条只收录具体Agent逆向辅助项目与APK调查用途，没有实测目标APK；REA协作是作者建议，未审实际联用轨迹。

候选封存0赞、10浏览、0转发、0回复；未安装项目或测量APK分析完整率。

## 来源

- [Johnson Li：仅APK时的Agent调用链与数据流调查，2026-11-15 20:03:03北京时间](https://x.com/i/status/2121937017642881334)
- [窗口前父回复：Graphite名称、仓库与REA协作建议，2026-11-15 00:19:46北京时间](https://x.com/i/status/2121639234293616957)
- [窗口前固定README：程序图、MCP、APK要求与静态局限，提交2026-11-14 13:53:37 UTC](https://github.com/johnsonlee/graphite/blob/d4dd8ee618b0345bb91de3f90c7c238b3f4425f9/README.md)

[English](en/graphite-apk-program-graph-agent-analysis.md) | [返回目录](../README.zh-CN.md)
