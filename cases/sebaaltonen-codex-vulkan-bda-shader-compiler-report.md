# Vulkan BDA着色编译器：Sebastian Aaltonen称Codex擅长逆向，指向GPU指针问题

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-10
阶段：待验证

2026年11月10日15:49:47（北京时间），Sebastian Aaltonen（@SebAaltonen）称Codex（Astra Ultra）擅长逆向，并说Intel与AMD的着色编译器bug和GPU指针、Vulkan BDA有关。BDA即Buffer Device Address，允许着色器通过设备地址访问缓冲区。这里收录的是作者将AI逆向能力与具体图形编译器问题相联系的短分析报告，不是通用模型排名。

作者进一步把DX／OpenGL的buffer抽象与Metal、CUDA、OpenCL的指针方式相对比，称Vulkan 1.3+两者都支持。这些API概括按作者表述保留，并未在此逐版本核对，不能据此断言某一API永无指针或所有驱动共有缺陷。原帖没有具体shader、输入输出、反汇编、提示、编译器版本、驱动、硬件或复现脚本，未展示Codex到底分析了哪段产物。

补取确认署名、正文和图片附件存在，未读取图片内容或被引用原帖，也未拿到issue、修复提交或厂商确认。bug一词不足以证明可利用安全漏洞、根因已定或修复交付；没有性能与跨厂商一致性测量。按作者分析待验证保留，REA未说明，未运行GPU工作负载或目标代码。

候选封存8赞、327浏览、0转发；无驱动版本、最小复现或独立验证。

## 来源

- [Sebastian Aaltonen谈Codex与Intel／AMD Vulkan BDA问题，2026-11-10 15:49:47北京时间](https://x.com/i/status/2120061340899541291)

[English](en/sebaaltonen-codex-vulkan-bda-shader-compiler-report.md) | [返回目录](../README.zh-CN.md)
