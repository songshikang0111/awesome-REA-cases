# ArtCraft：不要把从零开发写成逆向 Adobe

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-03
阶段：相关项目

ArtCraft官网描述用Rust从零编写创作软件，多款仍早期测试或开发，不能把传播帖当“已完整逆向Adobe”。WordCraft、GridCraft、DeckCraft分别重建Word式文字处理、Excel式表格和PowerPoint式幻灯片，提供相应Office格式与MCP，README仍标alpha。10月12日PhotoCraft材料称PSD基于Adobe公开规范，UI、CLI、JSON、MCP共用500多命令，309个psd-tools样本中307个打开再保存后渲染一致，不是所有文件字节相同；不构成专业日用Photoshop替代或Adobe反编译证明。

10月13日04:00–08:00窗口用户试用PhotoCraft，指出面板不能浮动、色彩管理不透明、保存缺少压缩等选项、PSD打开慢、图像焦点／蒙版读数及文字控制问题，认为不适合专业工作。这是单次体验，不是官方承认或本合集复现。10月14日第三方称PhotoCraft使用REA类流程，身份未确认，不算作者确认。10月15日转述又提公开格式规范、观察按钮、像素渲染比较及自制编解码器；20:48用户称Ubuntu上13个应用都能启动，并转述维护者在HN称团队不反编译、禁Ghidra、按公开信息与行为重建。启动不等于完整可用，HN原话、像素验证与编解码范围没有补查，不保证法律合规或全部套件兼容。

2026年11月3日23:44:34（北京时间）的新候选称试用Filmcraft，感觉与Adobe Premiere相同，并把整个ArtCraft说成Claude逆向所有Office和Adobe产品的成果。只将Filmcraft体验作为既有套件的新使用反馈；帖子没有版本、工程、编解码、效果或导出比较，“identical”是用户印象，不是功能等价或全部产品已被反编译的证据。没有独立研究方法、源码或新测试，仍保留从零重建／early-alpha边界，不另造整套逆向成功项目。未安装软件、运行用户工程或验证所有操作系统。

Office 补充发帖：2026-10-12T14:33:01+08:00（北京时间）
Office 补充帖热度快照（2026-10-12）：0 赞｜19 浏览｜0 转发
PhotoCraft 补充发帖：2026-10-12T16:08:50+08:00（北京时间）
PhotoCraft 补充帖热度快照（2026-10-12）：2 赞｜69 浏览｜0 转发
补充发帖：2026-10-13T05:58:20+08:00（北京时间）
补充证据：第三方具体使用反馈；未独立运行软件。
10月15日20:48新使用报告：发帖者称将官网13个应用装在Ubuntu，均可打开；这只是启动体验，不代表完整功能可用。他还转述维护者在Hacker News说不反编译二进制、团队禁止Ghidra，以公开信息和观察行为做clean-room重建。本合集未补查该HN原话，因此标明转述，不把启动、方法或法律边界升级为独立验收。
2026-10-14：第三方帖子称 PhotoCraft 使用 REA 类逆向工作流；发帖者身份未确认，非项目作者确认，未独立核验。
10月15日16:00–20:00窗口补充：新传播帖将公开PSD/Office规范、观察按钮行为、与Photoshop渲染逐像素比较列为重建路线，并声称自行实现视频编解码器。公开规范与从零实现不等于反编译Adobe；像素验证和编解码范围仍为该帖转述，不将其扩大为全部套件兼容、法律保证或本合集测试。其星数宣传不作为新热度快照。
11月3日Filmcraft候选快照0赞、16浏览、0转发；“像Premiere”仅为用户体验，没有功能对照。

## 来源

- [原始记录](https://x.com/iamdavidhill/status/2107248003543384170)
- [官网状态](https://getartcraft.com/apps)
- [本周期 WordCraft 介绍](https://x.com/realfxw/status/2109465865221550341)
- [WordCraft 项目与阶段说明](https://github.com/storytold/wordcraft)
- [本周期 Office 重建介绍](https://x.com/OLD9Gaming/status/2109532775170859138)
- [GridCraft 项目与阶段](https://github.com/storytold/gridcraft)
- [DeckCraft 项目与阶段](https://github.com/storytold/deckcraft)
- [本周期 PhotoCraft 文件互通与 Agent 控制介绍](https://x.com/i/status/2109556887645479114)
- [PhotoCraft 项目测试口径与 early alpha 边界](https://github.com/storytold/photocraft)
- [本窗口 PhotoCraft 第三方使用体验](https://x.com/i/status/2109765636750532915)
- [第三方帖子：称 PhotoCraft 使用 REA 工作流（发帖者身份未确认，非项目作者确认）](https://x.com/i/status/2110249246138245143)
- [10月15日本窗口的格式规范与验证流程转述](https://x.com/i/status/2110655957436965228)
- [10月15日20:48：Ubuntu安装体验与非反编译边界转述](https://x.com/i/status/2110714534591713611)
- [11月3日Filmcraft第三方体验与套件宣传，未验证等价](https://x.com/i/status/2117644109037085025)

[English](en/artcraft-boundary.md) | [返回目录](../README.zh-CN.md)
