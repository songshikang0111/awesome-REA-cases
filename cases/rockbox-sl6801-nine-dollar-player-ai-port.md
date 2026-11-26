# 9美元SL6801播放器跑Rockbox：AI研究原固件与低内存移植的转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-26
阶段：待验证

2026年11月26日04:58:06（北京时间）的短讯称开发者用Claude给无文档9美元AliExpress MP3播放器移植Rockbox，并报HN 160分、70评论，未提供可核HN页面。05:12:40，Embedded Systems（@embedsys）详细转述：Smartlink SL6801有两颗192MHz Cortex-M4、512KiB SRAM、2MB flash和无缓存XIP；codec与插件共用128KiB区域，启动插件会停止音乐，热点循环经profile后移到SRAM。最小既有目标2MiB是帖子比较口径，未核Rockbox目标历史。

方法据称是ghidra-mcp研究原FreeRTOS固件，用摄像头看屏、line-in听声音，通过双向USB开发shell注入按键和取截图，并运行数小时Python压力测试；驱动采用Ghidra研究者、裁判、实现者三角色重做。帖子称无需开壳、作者只略看代码且称100% vibecoded，又归功ilyakurdyukov发现ROM下载模式并写刷写工具。这些不是无人参与或法律净室保证；所谓发现上游bug没有提交与复现记录。

补充公开GitHub检索定位jaydens-tasty-slop/rockbox，仓库描述为YP3（SL6801）移植，固定master提交822b9f5e999122bc25738fc9746bb7a17bb48fa6时间为11月22日09:01:21北京时间，早于窗口；仅确认仓库身份、提交和根目录，未审实现，也没有读到根README，不能用仓库存在证明帖子所有参数与结果。它不同于既有给女儿10美元播放器重写固件的未实施idea。没有安装依赖、下载固件、执行代码或刷写；REA未提。

两候选封存依次0赞／11浏览／0转发／1回复、8赞／525浏览／2转发／2回复；HN热度仅短讯转述。

## 来源

- [Claude／9美元Rockbox移植短讯，2026-11-26 04:58:06北京时间](https://x.com/i/status/2125695546543243614)
- [Embedded Systems补充SL6801、研究方法与维护疑问，2026-11-26 05:12:40北京时间](https://x.com/i/status/2125699211169509405)
- [补充定位的YP3／SL6801公开仓库固定提交，2026-11-22，未审实现](https://github.com/jaydens-tasty-slop/rockbox/tree/822b9f5e999122bc25738fc9746bb7a17bb48fa6)

[English](en/rockbox-sl6801-nine-dollar-player-ai-port.md) | [返回目录](../README.zh-CN.md)
