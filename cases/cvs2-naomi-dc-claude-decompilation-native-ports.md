# Capcom vs. SNK 2：Claude辅助三版本反编译，字节匹配与跨平台移植分开看

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-26
阶段：待验证

2026年11月26日16:01:36（北京时间）的候选介绍gibletto的Capcom vs. SNK 2 v0.0.1：这款2001年格斗游戏的日美NAOMI街机版与日版Dreamcast程序据称100%字节匹配，另有Windows、Linux、3DS、PSP和MiSTer移植。它沿用Marvel vs. Capcom 2项目的工具与结构，但游戏目标不同，也不是基线Capcom vs SNK到SNES的计划。

补读公开仓库e3408908e9e9af696bada01e7281a5ac296282ef（提交于11月26日16:49:05北京时间）的根README与ports/README，属于候选之后的补充文档，不是另一条候选或本合集实测。根文档明确披露使用Claude，此时版本已写0.0.2。项目把三版机器码重写为C，原本汇编部分保持SH-4汇编；一套源码按版本条件编译。美国PS2版保留符号，提供约9700个例程名，结构体与字段等另行恢复／命名。文档报告日版街机约11300例程（其中约9800属Capcom、285文件），Dreamcast约15600例程、游戏部分358文件；字节一致不证明唯一原始源码，文档也承认部分匹配写法仍不自然。

构建文档列程序与镜像的预期SHA-1及检查步骤，不是本合集执行产生的哈希。街机大镜像复用自有游戏盘中的美术、声音等数据和8KB Z80代码；日版街机游戏程序链接300个SDK原模块、另建19个，Dreamcast链接467个、另建39个。不能把镜像字节一致解释为全部资源、库与辅助处理器代码都由AI恢复。原程序匹配构建还依赖特定Hitachi工具链及Sega SDK；使用者须合法取得相应材料，本合集不分发。

移植文档称直接编译游戏C并实现主机层，而音频仍有原驱动、ARM7／DSP模拟或C实现；原程序匹配不自动证明新主机行为或画面等价。PC使用SDL GPU的Direct3D12／Vulkan，Linux为32位x86；PSP仅Dreamcast版。Dreamcast网络无法连原服务器，串口Neo Geo Pocket连接与内置浏览器不可用，未实现库例程以stub记录。MiSTer文档承认部分透明排序像素差异；掌机等C音频模式可提前约1ms。候选的New 3DS全速、Steam设备支持等仍为宣传／项目口径，没有独立平台矩阵。已读固定文档，未审完源码、下载游戏、安装SDK、构建或运行任何移植；状态unverified，未提REA。

候选封存65赞、1550浏览、7转发、0回复；不以补查时热度或仓库存在证明匹配与移植完成。

## 来源

- [CvS2 v0.0.1、Claude参与及五平台移植的候选介绍，2026-11-26 16:01:36北京时间](https://x.com/i/status/2125862523215692261)
- [补充固定根README：Claude披露、三版本匹配与SDK／盘数据复用；提交2026-11-26 16:49:05北京时间](https://github.com/gibletto/cvs2-naomi-dc/blob/e3408908e9e9af696bada01e7281a5ac296282ef/README.md)
- [同一补充提交的移植文档：平台、主机层与声画／网络限制](https://github.com/gibletto/cvs2-naomi-dc/blob/e3408908e9e9af696bada01e7281a5ac296282ef/ports/README.md)

[English](en/cvs2-naomi-dc-claude-decompilation-native-ports.md) | [返回目录](../README.zh-CN.md)
