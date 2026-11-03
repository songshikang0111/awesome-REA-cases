# SpeakMore：REA研究Typeless后重写语音输入，离线与翻译能力须区分

分类：应用与客户端 · REA
记录日期：2026-11-03
阶段：进行中

2026年11月3日08:38（北京时间），一篇中文转述介绍B站作者用REA分析Typeless，形成18篇笔记，再独立写出SpeakMore，提供快捷键语音输入、去语气词、语音翻译和划词翻译。帖称Typeless年付144美元、日常使用SpeakMore月约1美元；这是转述的费用口径，不是本合集核价或成本实测。

补读zephyr4123/speakmore固定提交edb3ea8b3a1c6933347296f8a963dd529ca21a8b的README和Typeless总览；提交为10月30日21:31北京时间，早于窗口。文档对应同名产品、18篇笔记、macOS/Windows和MIT声明，并称根据交互独立实现、不含Typeless代码。它明确区分直出、混合和离线：离线本机模型只能转文字，不提供语音翻译；划词翻译始终走所选文字模型。费用按每天100次、每次26秒等假设估算，不能用转述的1美元概括所有配置。

总览称普通听写链路在10月13日做过四次抓包，并改正六处静态结论；翻译、HTTP兜底、修改跟踪、登录等仍未动态验证，服务端模型与提示词未知。客户端每3秒分块传输、WebSocket与HTTP兜底及上下文采集是项目研究报告，不证明已恢复服务端。README另自报1500单元测试、54安装测试，本合集未重跑、构建或审计最终包的隐私与签名。此具名公开实现不同于基线的REATypeless／Saydra，不强行合并。

候选快照2赞、241浏览、0转发；费用与测试为转述／项目自报，未独立复现。

## 来源

- [SpeakMore／REA与Typeless研究的中文转述，2026-11-03](https://x.com/i/status/2117415964367024205)
- [补充SpeakMore固定README，提交2026-10-30，早于窗口](https://github.com/zephyr4123/speakmore/blob/edb3ea8b3a1c6933347296f8a963dd529ca21a8b/README.md)
- [补充Typeless研究总览与动态验证边界，同一固定提交](https://github.com/zephyr4123/speakmore/blob/edb3ea8b3a1c6933347296f8a963dd529ca21a8b/targets/typeless/docs/00-overview.md)

[English](en/speakmore-rea-typeless-voice-input-report.md) | [返回目录](../README.zh-CN.md)
