# Apkscope：以Rust单程序与MCP连接Agent的APK研究工具介绍

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-14
阶段：相关项目

2026年11月14日06:53:27（北京时间），Big Bull（@BIGBULLapp）介绍Apkscope，称将Android APK研究集中到一个Rust可执行程序，避免传统流程中JVM、图形界面及dex2jar转换的切换成本。帖子列出带类型的Java反编译、交叉引用、API与secret线索侦察、APK差异、重签名、原生查看器，以及可让Agent使用同一分析能力的MCP服务。APK是Android应用包，MCP在此是Agent与分析工具的接口；相关项目的具体价值是给人工与AI提供共同的应用检查入口。

本条是工具介绍，不是已用某个可疑APK验证的案例。作者所称毫秒级反编译没有样本规模、设备、版本、计时方法或对照结果；没有取得短链指向的项目源码、许可证、文档或测试，不能核认完整功能、正确率或无JVM依赖范围。secret侦察指功能宣传，不表示已发现有效密钥，本合集未访问凭据、下载APK、重签名或运行程序。补取原帖确认署名及一张附图存在，未审图像；REA未提及，保留为Agent辅助逆向相关项目而非已复现成果。

候选快照1赞、16浏览、0转发、0回复；毫秒级是未核验宣传，不是本合集测量。

## 来源

- [Big Bull的Apkscope Rust／MCP APK工具介绍，2026-11-14 06:53:27北京时间](https://x.com/i/status/2121375920606847071)

[English](en/apkscope-rust-apk-analysis-agent-mcp-project.md) | [返回目录](../README.zh-CN.md)
