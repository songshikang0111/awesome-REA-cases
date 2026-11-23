# 逐镜视频分析进ComfyUI：Benji AI称把rea-video想法做成单节点

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-23
阶段：进行中

2026年11月22日19:41:15（北京时间），Benji AI（@AIfutureBenji）公告Shot-by-shot video reverse engineering Now In ComfyUI，并附视频。19:41:49同作者的后续帖进一步说明：将rea-video的idea做成单个ComfyUI自定义节点。ComfyUI是节点工作流环境；具体目标是将逐镜视频结构分析纳入已有工作流，而非要求用户另用独立视频分析入口。

这两条窗口前来源合为一个节点项目，不重复新增。此前补取同串确认署名、父子关系与1920×1080视频附件，但没有观看视频或取得代码、节点名、模型、输入输出schema、安装材料和测试。‘rea-video idea’是作者的灵感归因，不证明节点复用上游源码或直接调用morluto/rea。不能写成自动复刻完整影片、生成质量已验证或单节点覆盖全部视频制作。

11月23日05:26:00本窗口候选中，Prince does AI（@princedoesai）介绍Rea Video Breakdown for ComfyUI，称会将视频分镜、为每镜写提示，并特别称用光流测量运镜。补取原帖确认署名与图片附件，但未读图片或短链目标。作为相同ComfyUI逐镜分析目标的补充讨论归档；没有仓库、作者关系或版本标识来确认它与Benji所述单节点的精确对应，光流也仅为讨论者的功能描述，非已核源码或对照结果，不据此改写旧公告已实现的范围。保持in-progress；未安装节点或运行视频分析。

两条旧封存快照分别0赞／32浏览与1赞／15浏览；均0转发，回复分别1与0。附件存在不表示功能已复现。
11月23日新增讨论快照0赞、56浏览、0转发、1回复；光流、逐镜提示与版本对应未核。
2026年11月23日22:35:31（北京时间）新候选具名ComfyUI-ReaVideoBreakdown，称本地视觉语言编码器分析每镜、光流测pan速度和zoom率，输出VIDEO.md风格报告、JSON及中英文提示，不调用外部API，也不分析音频、读屏幕文字或导出字幕；普通SD1.5／SDXL CLIP不能看帧。MIT、两项依赖与功能均为转述，尚未核仓库、源码及与Benji版本的精确对应，未安装或运行。封存0赞、14浏览、0转发、0回复。

## 来源

- [Benji AI的ComfyUI逐镜分析公告，2026-11-22 19:41:15北京时间](https://x.com/i/status/2124468246489477576)
- [Benji AI后续说明单节点与rea-video idea，2026-11-22 19:41:49北京时间](https://x.com/i/status/2124468390576414723)
- [Prince does AI转述ComfyUI逐镜提示与光流测运镜，2026-11-23 05:26:00北京时间](https://x.com/i/status/2124615403095601301)
- [ComfyUI-ReaVideoBreakdown功能与缺项转述，2026-11-23 22:35北京时间](https://x.com/i/status/2124874492736577951)

[English](en/benji-comfyui-rea-video-shot-node-project.md) | [返回目录](../README.zh-CN.md)
