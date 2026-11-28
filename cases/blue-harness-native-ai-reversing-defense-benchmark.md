# blue-harness：给自有原生程序加固，以单次7B模型实验衡量AI逆向成本

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-28
阶段：分析测试

2026年11月28日06:15:16（北京时间），Python Hub（@PythonHub）推荐seifheakal/blue-harness，目标是让自有原生二进制与移动应用更难被AI辅助逆向，采用构建期审计、加固和验证。补读11月16日02:24:35北京时间的固定提交25a992255c1c766f4b1d8794d53c0027fbc73840：它扫描符号、字符串、熵与防护标志，提供ELF／PE／Mach-O的构建后加固和Claude skill，并以机制检查判断防护是否触发，不宣称软件不可破解。

README报告一次N=1前后实验：RTX 3070笔记本、8GB显存／16GB内存上运行4-bit量化7B模型；未保护样本在3步、1256 tokens、1.6秒内通过hash核验破解，加固样本13步、16785 tokens、195秒仍未破解。这是项目对自有CrackMe的单次测量，不是前沿模型、商业软件或多次统计的防御结论。文档明确honeytoken层在该次攻击中未触发，不能把单独机制测试当成该层已阻止LLM。

项目称362项检查通过，列出各防护强度与已知绕过；PE／Mach-O的部分构建期功能、Windows／Mac运行时证明以及Android／iOS内部覆盖仍有待办，不能从支持格式推出完整移动加固。不同段落的完成口径保留为项目文档，不替它统一成全面验证。本合集只读README，未检查全部原始运行记录、重跑实验或执行加固代码。此处是研究AI逆向成本的防御实验，未确认使用REA。

2026-11-28候选快照4赞、545浏览、0转发、0回复；实验与检查数字均为项目报告。

## 来源

- [Python Hub介绍blue-harness，2026-11-28 06:15:16北京时间](https://x.com/i/status/2126439740891091333)
- [补充固定README：单次7B测量与待办；提交2026-11-16 02:24:35北京时间，早于候选窗口](https://github.com/seifheakal/blue-harness/blob/25a992255c1c766f4b1d8794d53c0027fbc73840/README.md)

[English](en/blue-harness-native-ai-reversing-defense-benchmark.md) | [返回目录](../README.zh-CN.md)
