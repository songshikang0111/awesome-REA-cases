# MacBook9,1扬声器：Claude辅助识别CS4208数字路径与Ubuntu驱动适配

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-04
阶段：进行中

2026年11月4日02:23:45（北京时间），@jyz002发布Claude Code辅助的Linux互通笔记。目标是2016年12英寸MacBook9,1在Ubuntu26.04下无声的内置扬声器。作者称原生驱动和leifliddy项目使用模拟DAC，未走向四颗TAS5758L功放的数字路径；Weegee/macbook91-cs4208-pub已实现该路径，他将其与Ubuntu linux-source中的cs420x.c及local-changes.patch结合构建，安装独立模块并使其不进入initramfs。不是作者或Claude从零发明该驱动。

作者报告驱动需在原生驱动接触codec前读取开机固件状态，因而必须真正冷启动；没有硬件音量，使用WirePlumber固定-26dB上限，并在播放前以静音流数值核对满档增益0.050。所有sudo操作由作者亲自执行。原帖明确提醒未签名树外模块、扬声器可损坏与上游贡献困难。本合集完整读取原帖但未编译模块、播放声音、核验电气安全或其他机型；数字路径解释及增益测试均属作者报告，REA未提及。同帖NICOLA输入问题另列独立案例。

补读驱动README，固定提交03e7e4c12041cbf2c90b82e8a2f36000cafbecd9于11月2日，识别为面向Arch系的DKMS项目，本身明确署名Claude在维护者指导下写项目代码、测试与文档，并涉及Apple驱动分析。这是上游背景，不是jyz002的Ubuntu构建证明。项目区分历史实测、沿用与未运行结论：20261102.01未上硬件，内核7.3只编译，其功放I2C工具无法区分空地址与占用地址。本合集没有重跑这些项目测试。

候选快照1赞、25浏览、0转发；-26dB／0.050为作者值，不是本合集安全保证。

## 来源

- [@jyz002的MacBook9,1声音与输入笔记，2026-11-04](https://x.com/i/status/2117684171720233121)
- [补充驱动README：Claude署名、硬件测试边界，固定提交于2026-11-02](https://github.com/Weegee/macbook91-cs4208-pub/blob/03e7e4c12041cbf2c90b82e8a2f36000cafbecd9/README.md)

[English](en/jyz002-macbook91-cs4208-claude-ubuntu-speakers.md) | [返回目录](../README.zh-CN.md)
