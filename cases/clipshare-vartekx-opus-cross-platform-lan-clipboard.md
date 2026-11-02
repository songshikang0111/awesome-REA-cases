# ClipShare：vartekx用Opus做Mac／Windows／iPhone局域网剪贴板替代品

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-02
阶段：进行中

2026年11月2日07:12:49（北京时间），vartekx（@vartekxx）把ClipShare称作以Opus 5.5逆向Apple剪贴板的作品：希望Mac复制后直接在Windows粘贴，iPhone从网页参与，而不是靠聊天软件中转。作者称从空目录和“AirDrop, but between PC and iPhone”提示开始，由Claude Code选用Python标准库本地服务；iOS后台剪贴板受限，因此改用两个签名的Back Tap快捷指令。

作者报告40项端到端测试、40MB文件逐字节往返，称修复macOS全局广播发现失败、未配对前不能粘贴地址的引导死循环，以及两份进程各显示不同配对码的问题；改为自动发现、六位码配对并禁止重复启动。称一个晚上、自己零行代码、最终62KB两个文件，另做Vercel落地页与Remotion宣传片。这些是作者报告，不是本合集计时、源码计数或硬件测试。

补读同作者串中07:12:50的完整构建提示作为补充材料，不把它另算候选。提示要求Windows用ctypes调用Win32、Mac用pbcopy／pbpaste，同文件connect模式双向同步，iPhone使用Safari；要求流式文件最多2GB、请求密钥、每次启动更换配对码、五次错码锁一分钟、过滤系统标记的私密剪贴板及只存内存历史。这些是需求，不是已审计的实现。提示明确LAN使用明文HTTP、限家庭Wi-Fi，不能把“无云”写成传输加密或安全保证。40MB自测也不能证明2GB上限可用。

只查原帖与作者串，未解析仓库短链、阅读源码、观看演示或运行服务；未接触真实剪贴板、密钥或配对。所述普通系统接口支持功能替代的解释，没有证据证明恢复了Apple通用剪贴板／AirDrop私有协议，也不保证所有系统自动后台同步。

候选快照12赞、324浏览、0转发；40测试、40MB、一个晚上、62KB与两个文件均为作者自述。
2GB、密钥、私密标记过滤与锁定是构建提示要求，未经源码或安全验证；LAN明文HTTP。

## 来源

- [候选：vartekx的ClipShare制作、测试与配对排错报告，2026-11-02](https://x.com/i/status/2117032140009594890)
- [补充同作者串：完整构建提示与明文HTTP边界，2026-11-02 07:12:50](https://x.com/i/status/2117032145139204569)

[English](en/clipshare-vartekx-opus-cross-platform-lan-clipboard.md) | [返回目录](../README.zh-CN.md)
