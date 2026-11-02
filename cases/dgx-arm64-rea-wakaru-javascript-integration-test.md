# DGX ARM64的REA／Wakaru：JavaScript恢复工具接线与回归自测

分类：应用与客户端 · REA
记录日期：2026-11-02
阶段：分析测试

2026年11月2日20:41（北京时间），发帖者贴出AI工作回执：在DGX安装Wakaru 1.14.0 ARM64，把REA 6.4.0的仅x64架构门扩为x64／arm64并重编译，两个启动器导出Wakaru命令；Mac mini的DeepSeek转发层将REA可用工具从8扩为10，加入analyze_javascript_application与recover_javascript_sources。称修改仅有本地提交0306f44，未推送。目标是在ARM64机器让AI调用JavaScript分析与恢复流程。

回执自报：131835字节React DOM 18 UMD单文件恢复exit 0，产出1模块及source map，用时230ms；Babel parser目录经rea-javascript-application分析成功；Ghidra分析系统ls回归成功。MCP列出170工具含两个JS工具，转发层测试2/2通过。全量测试有team-report.test.js找不到bin/cdx的一项失败，回执称修改前已存在，未独立核对此前状态。

工具只对新DeepSeek会话生效，当前会话仍8个；REA升级或重装会覆盖本地修改。回执称新增约23MiB、探针约9MiB，浏览器CDP相关analyze_web_bundle未放行，实测新会话仍是下一步。没有公开补丁、输出文件、source map质量比较或原始测试日志。成功退出不证明恢复了原始源码，也不是所有JS包支持；本合集未安装、执行或访问作者机器。

候选快照1赞、59浏览、0转发；版本、字节数、230ms、工具数和测试结果均为贴出的回执，未独立复验。

## 来源

- [DGX ARM64的REA／Wakaru适配与自测回执，2026-11-02](https://x.com/i/status/2117235562981523901)

[English](en/dgx-arm64-rea-wakaru-javascript-integration-test.md) | [返回目录](../README.zh-CN.md)
