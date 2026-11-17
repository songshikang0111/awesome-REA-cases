# zniff：Rust抓包工具以MCP让Claude和Cursor查流、重放与改规则

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-17
阶段：相关项目

2026年11月17日21:12:56（北京时间），vicanso（@tree_xie）宣布zniff开源。目标是HTTP(S)流量观察、协议调试与规则修改，并把这些能力通过内置MCP交给Claude、Cursor。它是供AI研究应用通信的具体基础工具，不是已报告破解某个服务。

作者称Rust代理核心与NSH原生跨平台UI可打包为单一二进制，也可编译WebAssembly，提供网页／Docker远程控制台。列出的协议包括HTTP/1.1、HTTP/2的ALPN协商、WebSocket、SSE；解码包括JSON、GraphQL、无模式Protobuf/gRPC、MessagePack与行内字段，并有Diff、瀑布图、时序图。作者还列15项改写规则与断点、多语言代码导出，MCP可查流、重放和改规则。保留为产品能力自述，不保证任意加密流量可解密或所有协议无损。

已核对原帖作者与文字，未检查仓库、许可、代码、捕获样本或MCP会话，未安装代理、证书或目标依赖。没有性能或内存测量，不把告别Electron的表述当比较基准；REA未提及，状态为相关项目。

2026-11-17封存2赞、45浏览、1转发、1回复；15项规则为作者列举，未经逐项核验。

## 来源

- [vicanso发布zniff及MCP能力，2026-11-17 21:12:56北京时间](https://x.com/i/status/2122679379734253648)

[English](en/zniff-rust-mcp-http-traffic-research-tool.md) | [返回目录](../README.zh-CN.md)
