# Yoda Stories：Ghidra配Claude转写引擎，字节匹配暂停、SDL仍在推进

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-20
阶段：进行中

2026年11月20日22:01:51（北京时间），whyamas（@whyamas）介绍@ShinyQuagsire让Claude在Ghidra和计划文件基础上主导Yoda Stories引擎反编译，称README报告全部转成C++、SDL移植进行中。补查shinyquagsire23/Yodecomp的850368bc1727dcf2f690d78b10fc1fcd1c09f453，提交为9月9日11:36:13北京时间，属于窗口前项目文档补证，不是11月新增完成。

README报告100%引擎转写为惯用C++并能从源码构建EXE，但Claude因字节匹配反复停滞而暂停匹配，正在通过替代MFC及部分GDI的microfx移植SDL。100%是转写范围自述，不能改成100%字节匹配或已验证完整游戏等价。构建需自备游戏资产与工具链，本合集没有取得资产或构建。

作者说明给Opus游戏资产、Ghidra中已加载的Yodesk.exe、经MCP／curl访问的反编译器、OpenJKDF2与DesktopAdventures参考和CLAUDE.md计划；所引计划又写YodaDemo.exe，保留文档不同目标名，不擅自统一。他大多让Claude推进，但亲自纠正过度自信且错误的命名，要求把结构写回Ghidra而非仅存Markdown，并手工驱动可空上下文接续的阶段协议，偶用Fable。它不是无监督自动循环。只读README，不审全部源码、视频或测试日志，不确认C++转写和SDL版所有路径可用；REA未提及。

候选封存0赞、5浏览、0转发、0回复；100%转写是项目报告，不等于字节匹配，手工监督与匹配停滞均保留。

## 来源

- [whyamas介绍Yoda Stories／Claude，2026-11-20 22:01:51北京时间](https://x.com/i/status/2123778852669554700)
- [补充：Yodecomp固定README，2026-09-09 11:36:13北京时间](https://github.com/shinyquagsire23/Yodecomp/blob/850368bc1727dcf2f690d78b10fc1fcd1c09f453/README.md)

[English](en/yoda-stories-ghidra-claude-engine-transcription.md) | [返回目录](../README.zh-CN.md)
