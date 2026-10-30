# xmen2-pc：Claude Code辅助重建《X战警2》，扩展四人回滚联机

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：进行中

2026年10月31日02:36:57（北京时间），The Gaming Emporium（@McGroin83）介绍crabsmack的xmen2-pc，把1995年Sega Mega Drive／Genesis的X-Men 2: Clone Wars原生移植到Windows与Linux，加入四人本地／在线合作、回滚网络、宽屏和高刷。帖文明确披露，开发者称几乎整个项目由Claude Code Agent写成。补读固定提交06783ee115f1e374d35bf088ce432cfa962d5739的README；2026-10-28T01:40:12Z提交早于窗口，仅作项目补证。

README把工作拆成字节匹配反汇编、基于segagenesisrecomp的静态重编译、确认原编译器Apple MPW C3.3、可读C重建、去掉68000模拟的原生移植，再到增强和联机。项目称3164函数中3047个原C函数用原编译器编成卡带相同机器码；另117个原汇编函数无法由C编译器字节匹配，采用逐指令对照重编译代码，报告无差异。关闭选项时测试运行逐帧状态和画面一致，但刻意不重现原卡带掉速；这些都是项目报告，不是本合集重算的匹配率或全输入等价证明。

项目称几乎全部由Claude Code在九天内、按可测完成标准实现；REA未提及。16:9视图与改变敌人激活范围的widescreen_gameplay分开；high_fps靠原帧间插值支持61至1000Hz，不是加速游戏逻辑；full_rate_2p把原来减半的双人逻辑恢复60帧。新增三／四人模式明确玩测较少。在线每人须持自己的ROM、同一release，v1.1.0拒绝v1.0.x；网络效果未在这里实测。

只接受USA／Europe兼容ROM，资产启动时从用户文件读取，项目不提供卡带内容。原创代码MIT但所依赖segagenesisrecomp为PolyForm Noncommercial，README说明移植构建不可商用，不能笼统称整个产物可商用MIT。未下载ROM、执行目标、安装依赖或重跑编译／差分测试；以公开实现与明确自测边界收录。

候选快照1赞、194浏览、0转发；九天、3047／3164及117函数无差异均为项目报告。
固定提交早于窗口；四人新功能测试较少，未独立运行游戏或校验匹配。

## 来源

- [The Gaming Emporium介绍xmen2-pc，完整原帖含Claude Code披露，2026-10-31 02:36:57](https://x.com/i/status/2116237941227843747)
- [补充：10月28日固定README，字节匹配、联机与许可边界](https://github.com/crabsmack/xmen2-pc/blob/06783ee115f1e374d35bf088ce432cfa962d5739/README.md)
- [补充：10月28日文档提交及Claude Opus协作署名](https://github.com/crabsmack/xmen2-pc/commit/06783ee115f1e374d35bf088ce432cfa962d5739)

[English](en/xmen2-pc-claude-genesis-native-port.md) | [返回目录](../README.zh-CN.md)
