# RDNA着色器研究idea：Sebastian Aaltonen建议经SPIR-V转源码再让AI命名变量

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-08
阶段：进行中

2026年11月8日22:06:45（北京时间），Sebastian Aaltonen（@SebAaltonen）讨论GPU着色器逆向：他说最新AI编写的PS5模拟器可把AMD RDNA指令集转换为SPIR-V，分析者可复用开放工具，再转为HLSL、GLSL或Metal，最后请AI给变量命名。目标是把较低层GPU指令转成更便于人读的着色器表达，以辅助理解既有渲染逻辑。

这是有明确转换链的研究idea，不是作者报告已对某款游戏或着色器完成恢复。原帖没有模拟器仓库、版本、反编译器、shader样本、输出、变量命名评估或语义等价验证；其关于AI编写模拟器的说法也仅归因作者。转换与可读命名不等于恢复原始源码、变量名或完整图形管线。

11月9日补取确认署名和措辞；按早期想法保留，不用进行中标签冒充已有实现。未下载或运行工具，REA未提及。

候选快照1赞、82浏览、0转发；idea，无具名shader验收。

## 来源

- [Sebastian Aaltonen的RDNA／SPIR-V／AI命名研究建议，2026-11-08](https://x.com/i/status/2119431434179858519)

[English](en/ps5-rdna-spirv-ai-shader-variable-recovery-idea.md) | [返回目录](../README.zh-CN.md)
