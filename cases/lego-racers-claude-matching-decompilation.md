# LEGO Racers：Claude署名提交参与1999年游戏的匹配反编译

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-20
阶段：进行中

2026年11月20日16:30:12（北京时间），yibie在列表更新中介绍isledecomp/racers，称1999年LEGO Racers重建为匹配C，最近30次提交有188处AI commit trailer。补读项目README与提交后，确认它是面向原版LEGORacers.exe和GolDP.dll的进行中反编译，用Visual C++6.0生成代码并以reccmp比较原始机器指令，目标是可修改和后续移植的代码库，不是单纯从截图重做游戏。

固定提交7675cebe85578e529d384bc3a5a47ac6163cb553原始日期11月13日23:38:41北京时间，早于本轮窗口，仅作补证。其合并消息多处署名Claude Fable5.2，报告BeamEntity::Draw由72.41%到100%、PlayerControls::UpdateSteering由83.80%到100%，也记录仍不足100%的碰撞与渲染函数。署名能表明特定提交的AI参与，不能量化全项目贡献；188处为列表作者统计，未独立复算，也不等于188次独立提交。

同版本README称主执行文件几乎全部反编译、GolDP大部分完成、重编译游戏可玩但软件渲染器尚不可用；本仓库仅面向32位Windows，现代跨平台版本另属racers-portable，不混为本项目成果。没有运行编译器、游戏或reccmp，未验证整文件一致性、可玩性或原始源码唯一性。REA未提及，状态保留in-progress。

候选封存0赞、153浏览、0转发、0回复；112星与188处trailer为转述快照，未独立复算。

## 来源

- [yibie的两个游戏项目列表更新，2026-11-20 16:30:12北京时间](https://x.com/i/status/2123695393049604396)
- [补充：11月13日固定提交的项目README](https://github.com/isledecomp/racers/blob/7675cebe85578e529d384bc3a5a47ac6163cb553/README.md)
- [补充：Claude署名与具体函数匹配改善的合并提交，2026-11-13](https://github.com/isledecomp/racers/commit/7675cebe85578e529d384bc3a5a47ac6163cb553)

[English](en/lego-racers-claude-matching-decompilation.md) | [返回目录](../README.zh-CN.md)
