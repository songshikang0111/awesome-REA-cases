# 0安全harness：多模型二进制研究、并行复现与补丁验证的发布转述

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-09
阶段：相关项目

2026年11月9日01:02:19（北京时间），@Peak__Twilight介绍@0securitylabs的0项目，称是开源AI安全harness，支持多模型、逆向、Web界面、CLI与MCP，由并行Agent调查、复现漏洞并测试修复，覆盖Web/API到二进制与内核。目标是把调查、证据、复现和补丁接成工作流。该帖还声称30余Linux内核零日、影响运行于30多亿设备的软件，提及瑞士、意大利、欧盟政府代码、Wireshark、node-forge、jsonata与YC F26；这些缺少漏洞/披露清单、上游修复或融资记录，不作确认。

11月9日19:43:15，心有猛虎（@zg0820）转述0sec Labs在11月8日发布研究预览，MIT/Apache-2.0双许可，模型自带，可接OpenAI、Anthropic、DeepSeek、Kimi、GLM、Grok。他说五个面为Web、源码、依赖、二进制与内核；二进制内嵌0verse，封装Ghidra、angr、AFL++。Web路径shell优先使用bash、curl、python3、sqlmap，证据从candidate到impact-proven分级，并要求独立会话在五轮内再触发才确认，否则不升级。补取确认发帖者和全文，未读原架构文档、许可或固定实现，以上均为该帖的具体项目说明，不是本合集运行。

新帖明确XBOW Web CTF的93/95是any-success分组自报，黑盒union口径81/104，2026年某次冷启动45/104。三种设置、分母与成功聚合不同，不能相加、拿97.9%泛化逆向正确率或比较为同环境回归；没有原始样本、模型/版本、预算和逐项日志。11月8日是转述的发布日期，冷启动精确日期未给，不把本次报道当新测试。

始终没有项目固定代码、CVE、有效漏洞复现或补丁测试。独立会话是harness内的验证策略，不等于本合集独立验证；扫描、候选和补丁生成也不自动成立零日。REA未提及，本合集未安装、启动Agent、扫描或执行目标。

较早封存9赞、713浏览、2转发；30余零日及30多亿设备为无清单主张。
19:43候选封存1赞、24浏览、0转发；基准、11月8日发布和许可均为二手说明，未审原记录。

## 来源

- [Peak__Twilight对0securitylabs多模型安全harness的发布介绍，2026-11-09](https://x.com/i/status/2119475616030630059)
- [心有猛虎转述0verse、复现门槛与不同基准设置，2026-11-09 19:43:15北京时间](https://x.com/i/status/2119757707238580592)

[English](en/zero-security-labs-multimodel-reversing-harness.md) | [返回目录](../README.zh-CN.md)
