# KachraClean：REA黑盒研究CleanMyMac，补上开发依赖与模型缓存清理

分类：应用与客户端 · REA
记录日期：2026-11-03
阶段：进行中

2026年11月3日12:34（北京时间），Nikhil Deshpande（@nikhdesh）发布KachraClean 0.1.5：商业清理器只提示17.6 GB，而开发项目与模型占掉更多空间。他报告在120个依赖／构建文件夹中找到43.9 GB，模型缓存另有70.9 GB；这些是单台Mac的候选大小，不是已经释放的容量，也不意味着全部可删。

补读公开仓库固定提交940a2f656d5fa82d8c30c66774ec1555e75cf17c（11月1日14:12北京时间）。README与10月17日至11月1日研究日志早于本窗口，只作本次新报告的补充证据。日志明确目标是CleanMyMac 5.7.2，使用REA 6.5.0与Claude Code；作者设定不反编译代码、不解密规则库，观察包元数据、UI与运行行为后写自己的规格。1,343,066次事件来自用户用fs_usage记录、另用Python分析，不是REA自动抓取；REA的UI helper冷编译超过60秒导致超时，作者编译同一helper作读取绕行，人点击、Agent观察。净室是项目自定流程，不是本合集法律认证。

日志报告约2.5分钟参考扫描、107线程；单次无特权helper的观察不能覆盖所有模块。后续用Spotlight元数据推测未使用应用判定，并在看到筛选结果前预测四个应用，作者称四项都命中。实现为Swift核心、CLI与SwiftUI界面：只读扫描，逐项给safe／review／risky及理由，回收站删除与内存内Undo。撤销不持久化，重启／崩溃后不能依赖；日志记录过清理时崩溃丢失内存Undo，称0.1.4修复。

11月1日安全记录还承认旧报告可伪造模型项、借Full Disk Access移动任意用户文件，以及调用可写目录docker二进制的问题；0.1.5称增加每类清理时校验、旧报告不预选、限制签名Docker CLI，测试从38增至46。属于项目修正与自测，没有在本合集重跑。Docker只对记录输出测试，非实机；README的约78 GB缺口与发布帖较后细分不可混成同次测量。macOS 14+、无Apple开发者账户、ad-hoc签名且未公证；未下载应用、执行清理或独立验证安全和等价性。

11月3日候选快照1赞、129浏览、0转发；17.6／43.9／70.9 GB和46项测试均为作者／项目口径，非本合集复现。

## 来源

- [Nikhil发布KachraClean与REA黑盒研究，2026-11-03](https://x.com/i/status/2117475470036148719)
- [补充README，固定2026-11-01提交，早于窗口](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/README.md)
- [补充研究与安全日志，2026-10-17至11-01，固定提交](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/case-study/log.md)
- [补充扫描行为规格，单次无特权helper观测](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/spec/01-scan-behavior.md)
- [补充清理分类规格，保留未测模块边界](https://github.com/nikhilrdeshpande/KachraClean/blob/940a2f656d5fa82d8c30c66774ec1555e75cf17c/docs/spec/02-cleanup-categories.md)

[English](en/kachraclean-rea-blackbox-mac-cleaner.md) | [返回目录](../README.zh-CN.md)
