# VIctory兼容研究：AvatarManz分支的Claude归因、单机性能与图形缺陷

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-27
阶段：待验证

2026年11月26日20:19:02（北京时间），添财（@BitTheOnly）介绍Victory的Xbox到PC兼容研究，转述AI加快API与图形工作、显示开场和序章、人物车辆建筑可见但着色器与纹理问题严重；参与者预计48小时内初步可玩。此前确认署名、全文和视频附件，未观看或运行；48小时是预测，不能认证可玩或项目总工时。帖中Leonida终止说法不裁定该项目的冲突材料。

11月27日07:17:00，Ai神经猿（@Shenjingape）又称Claude与Gemini参与实验性Xbox模拟器，帧率一天从3至5升到25至30，AvatarManz的176次提交中171次由Claude署名，某版连续41分钟不崩，并转述Take-Two对相关仓库发出DMCA。原帖未附计数查询、具体修订、硬件、运行日志或通知，不能把这些数值、法律状态及官方PC发售传闻作为已核事实。

本轮补查公开仓库avatarmanz/VIctory-7900XTX，固定014d52dedf837d1ac660a0bd256c4704be9eeb40，提交时间11月27日06:33:21北京时间，作为补充材料而非新候选。README标日期11月26日，说明是Marvisak/VIctory兼容层的分支，起自fxceless分支，并列DexNom、Belobug等上游贡献；明确本分支修改使用Claude Code，最新提交说明有Claude Opus 5.5共同署名。这里证明公开归因，不是171／176的统计核验，也不证明Gemini用于本分支或全由模型独立完成。保留既有Victory ID，不为这个具名分支另开目标；文档显示与Belobug存在贡献关系，但不能因此把所有旧演示和作者合并成同一版本。

项目目标是在RX 7900 XTX上先恢复Series X画面正确性，再达到开光追30FPS以上，之后降内存需求；文档自称porting而非emulating，以修补原渲染器行为及预翻译着色器减少共享内存复制。单机配置Windows 11、i9-12900K、64GB RAM、RX 7900 XTX，城市站立／走动各270秒报告：4K输出、1440p绘制开光追约10／9FPS、45GB RAM；同画幅关光追约20／16FPS；1080p输出关光追约25／23FPS、42GB RAM；Series S关光追约23／16FPS、37GB RAM。这不能概括成所有模式25至30FPS或已达30FPS目标。旧表另列同场景补丁前57至75ms、关光追约22FPS、25790／25985着色器翻译且其余为未用geometry shaders，均为项目报告，不证明全游戏正确。

文档报告修正树木短暂消失与部分室内灯光问题，但仍列远景闪烁、纹理／模型细节加载慢、移动物体光追结构损坏（约450个异常指针／帧）、新构建管线卡顿，以及记录游戏帧会触发看门狗。最新提交又报告其它场景时延变化，不合并成统一性能结论。只读固定README和提交说明，未审完整补丁、日志或重跑；此前未取得仓库的限制仅在此范围解除。仓库声明不含游戏文件，需自备副本，本合集未审资产政策、认证合法来源、获取游戏／密钥或执行目标；未提REA，保持unverified。

旧候选封存6赞、1711浏览、0转发、0回复；48小时与启动画面未经独立核验。
新候选封存1赞、257浏览、0转发、0回复；171／176、41分钟、25至30FPS及DMCA均为未核二手说法。
固定README只报告一台RX 7900 XTX机器；设置、场景与日期不能混合，公开署名不是全部代码或测试的独立审计。

## 来源

- [添财转述Victory的AI兼容研究、序章画面与缺陷，2026-11-26 20:19:02北京时间](https://x.com/i/status/2125927306569130432)
- [Ai神经猿转述AvatarManz、帧率及Claude署名，2026-11-27 07:17:00北京时间](https://x.com/i/status/2126092889000132767)
- [补充固定VIctory-7900XTX README：11月26日文档、单机数据及Claude Code归因，版本提交11月27日06:33:21北京时间](https://github.com/avatarmanz/VIctory-7900XTX/blob/014d52dedf837d1ac660a0bd256c4704be9eeb40/README.md)
- [同固定提交说明：场景时延与Claude Opus 5.5共同署名，未审完整补丁](https://github.com/avatarmanz/VIctory-7900XTX/commit/014d52dedf837d1ac660a0bd256c4704be9eeb40)

[English](en/victory-gta6-ai-pc-compatibility-secondary-report.md) | [返回目录](../README.zh-CN.md)
