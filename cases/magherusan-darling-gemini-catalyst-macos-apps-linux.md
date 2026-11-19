# Darling运行Notes与iMessage：Gemini提示Catalyst后，进程启动但仍不可用

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-19
阶段：进行中

2026年11月19日21:30:42（北京时间），Cristian Măgherușan-Stanciu（@magheru_san）报告在Linux用Darling运行macOS原装应用（Notes、iMessage等）的进展。Darling是macOS应用的Linux运行兼容环境，不是把整个macOS虚拟化。补读项目README确认这层背景；README未用于验证作者的具体应用实验。

作者说Claude额度耗尽后改用其称为Gemini Argon的模型，模型指出这些应用的Catalyst／UIKit依赖，而不是他和Claude原先着眼的AppKit／Cocoa。把线索告诉Claude Opus后，已推进到应用进程启动、创建SQLite数据库，但要变得可用还缺多项服务，需在Darling中实现。框架判断为作者对所测应用的说法，不扩展到所有macOS应用。

没有应用与系统版本、补丁、启动日志、数据库记录或功能测试，不能写成Notes或iMessage已可用。模型名称保持作者原话，未独立认证。原帖署名已读，未构建Darling或运行Apple程序；REA未提。同帖的共享剪贴板为另一目标，另立记录。Darling未固定版本README于11月20日补读，原始发布日期未确定，只作补充背景，与窗口候选分开。

## 来源

- [Cristian的Darling／Catalyst与AI研究自述，2026-11-19 21:30:42北京时间](https://x.com/i/status/2123408626203111602)
- [补充背景：Darling README，2026-11-20阅读，未固定版本、原始发布日期未确定](https://github.com/darlinghq/darling/blob/master/README.md)

[English](en/magherusan-darling-gemini-catalyst-macos-apps-linux.md) | [返回目录](../README.zh-CN.md)
