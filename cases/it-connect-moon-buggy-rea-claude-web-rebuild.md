# Moon-Buggy：Florian BURNEL用REA与Claude读二进制并重建网页游戏

分类：游戏与游戏保存 · REA
记录日期：2026-10-30
阶段：分析测试

本轮2026年10月30日01:01:38与01:30:29（北京时间）的两个候选转发Florian BURNEL的IT-Connect文章。补读原文标注2026年10月29日，是较早发布的补充材料，不冒充本窗口首发。作者选择Jochen Voss于1998年创建的GPL开源ASCII游戏Moon-Buggy，以Linux Mint虚拟机里APT安装的stripped x86-64 ELF为输入，称不看源码进行分析；因此这是有公开源码可供事后对照的教学测试，不是破解闭源游戏。

作者要求Claude Code的Opus5.5通过REA找出滚动、跳跃、障碍、计分和碰撞规则，并为结论提供地址、指令或常量及未解项，随后生成单文件index.html。报告称程序有97个无名函数，Agent从score_crater、level_start等字符串追踪引用，调用Ghidra分析13个车辆精灵与8关表等结构；从分析到网页版本共12分29秒。文中列每列0.08秒滚动、五态跳跃共1.08秒且离地0.88秒/最高两行、宽1至6的坑、需三次激光命中的障碍，以及跨障碍+20、击毁+13、每射击-1等规则。

BURNEL声称核对后这些规则都正确，但模型称为岩石的对象在源码中是陨石；网页可用键盘玩，并提到独立ANALYSE.md保存地址证据。本次读到的是文章和其中展示的过程，未取得完整分析报告或运行HTML，也未独立测量时长、逐条验证地址、复算游戏规则。文章说无REA也可做类似工作，但未给受控计时对照，不能据此计算加速倍率。社区DX-Ball、ReaCut、VSL-DSP只是已有项目背景，不归于本次作者的Moon-Buggy实验。

两候选快照分别0赞/11浏览/0转发与5赞/460浏览/0转发。
12分29秒及规则正确性为作者报告；本合集未重跑，未取得完整ANALYSE.md。

## 来源

- [候选转发IT-Connect测试文章，2026-10-30](https://x.com/i/status/2115851565202382949)
- [同窗口转发并明确署名Florian BURNEL，2026-10-30](https://x.com/i/status/2115858824032596199)
- [补充：Florian BURNEL的Moon-Buggy完整教学测试，原文日期2026-10-29](https://www.it-connect.fr/rea-retro-ingenierie-ia-ghidra/)

[English](en/it-connect-moon-buggy-rea-claude-web-rebuild.md) | [返回目录](../README.zh-CN.md)
