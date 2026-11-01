# GameFrame：转述REA／Ghidra／Unicorn旧游戏重建技能链与POD测试边界

分类：游戏与游戏保存 · REA
记录日期：2026-11-01
阶段：相关项目

2026年11月1日10:58:41（北京时间），一篇阿拉伯语／英语帖子介绍GameFrame，为人和编程Agent理解、逆向与重建旧游戏提供技能，关注缺乏文档的遗留系统与逻辑。14:30:11的新介绍补充了具体流程：从自己拥有的游戏拷贝出发，依次清点文件、观察运行、反编译、跟踪调用、解析格式、模拟执行、重新实现、验证并合并，称使用Ghidra、Unicorn和REA，每步测试并与原版对照。

新帖列8／16位家用电脑、NES至第七世代主机、Game Boy至Switch掌机、街机，以及id Tech、Build、Unreal、Flash；这些是宣称的框架范围，不是逐平台验收清单。重建版据称共用带启动器、游戏库、设置、渲染器切换、帮助页与事件控制台的外壳。针对90年代末Windows加速卡游戏，介绍还列Glide 2、PowerVR SGL、ATI3DCIF、S3D Toolkit及DirectDraw替身DLL，但明确目前只在Wine下用POD测试过。

安装介绍称把设置提示词交给Claude Code、Codex或Cursor后，Agent先检查环境、安装前询问，再跑Ghidra测试、注册REA并建项目；称代码Apache 2.0、不带游戏文件，游戏本体、提取资源和反编译代码不得提交仓库。另提醒Claude Code的现有游戏复刻限制可能拦截流程；这是报道中的兼容性提醒，不是本合集验证供应商所有政策。

此前公共搜索未找到可确认的同名仓库，本次没有取得固定源码或POD测试记录，故不把其他Unity框架或LED项目嫁接过来，也不把技能步骤等同成功重建游戏。REA归类依据新介绍，不是实际调用日志；本合集未安装技能、获取游戏资产或运行测试。

较早候选0赞、12浏览、0转发；新增候选1赞、221浏览、0转发。
未读固定实现或测试记录；宽平台范围与Apache 2.0均为介绍说法，POD不是全部游戏验收。

## 来源

- [GameFrame旧游戏逆向与Agent技能项目介绍，2026-11-01](https://x.com/i/status/2116726591761821933)
- [新增介绍：技能顺序、REA工具链及仅Wine／POD测试边界，2026-11-01 14:30](https://x.com/i/status/2116779819526713673)

[English](en/gameframe-legacy-game-agent-reconstruction-skills.md) | [返回目录](../README.zh-CN.md)
