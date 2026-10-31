# Sonic Adventure日版：Claude与Codex辅助Dreamcast匹配反编译及GCC移植

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-01
阶段：分析测试

2026年11月1日03:49:53（北京时间），Kyle Mayer（@kylemayer）称四周持续用Claude Code与Codex完成原始日版Sonic Adventure的Dreamcast字节匹配反编译，约一百万行C，并花数百小时人工打磨，之后将SuperH C移植到现代GCC。他感谢Falco Girgis的SH4ZAM手写SH-4数学库。首次完整Dreamcast匹配项目、行数与工时均是作者说法，不是本合集测量。

补查公开reshaped/sonic-adventure的固定提交25a3d3154dbe657325e97dbe8c5291086f6af5c0（2026-10-31 17:16:28 UTC，即候选前的项目文档）：目标明确为HDR-0001、1.007版，README报告247个二进制、5820458代码字节，97.7% C、2.3%汇编；14份C源码需要shckit修补编译器汇编。匹配构建用Hitachi SHC、光盘数据与地址表恢复二进制，每个输出与原盘比较；不带光盘的make check只检查可链接源码的记录哈希，不生成完整二进制。GCC16.2路径重新链接映像，另提供默认关闭的16:9、60fps和帧计数器，不等于Windows／Linux原生游戏移植。

字节匹配不能证明恢复原始源码文本或原构建设置。须自备合法日版光盘；README只为构建工具与测试等部分声明MIT，其余仓库无许可证。这里仅阅读原帖与固定文档，未下载光盘、安装工具链、运行项目或重算匹配结果。

候选快照0赞、32浏览；未独立构建。
247个二进制／5820458代码字节为项目报告；匹配路径与GCC路径不同。

## 来源

- [Kyle Mayer的Claude／Codex反编译报告，2026-11-01](https://x.com/i/status/2116618684773158965)
- [补充一手：候选前固定提交README，匹配范围、GCC路径与许可](https://github.com/reshaped/sonic-adventure/blob/25a3d3154dbe657325e97dbe8c5291086f6af5c0/README.md)

[English](en/sonic-adventure-dreamcast-claude-codex-decompilation.md) | [返回目录](../README.zh-CN.md)
