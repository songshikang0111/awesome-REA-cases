# LDraw Mecha：从乐高零件文本推机构，再映射到Blender动画

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-08
阶段：相关项目

2026年11月8日05:17:00（北京时间），Xiao Tan（@tvytlx）介绍antelocnova的LDraw Mecha：用零件描述和位置文本推断机械子模块及联动，把注释映射到glTF节点，再用Blender Python绑定和动画。目标是让既有静态乐高CAD模型的机构动起来，不是单纯从提示生成新积木。候选举42043卡车太复杂，Claude Sonnet提议只做气动起重机；作者接受缩小范围。

补读该帖所链Show HN原作者说明（原发2026年11月7日03:41:20北京时间），确认公开仓库anteloc/ldraw-mecha与v0.5.0。读取该标签README、Gallery及validation文档；GitHub API给出提交c09ad90caf4f4cba00b1542eb622de8e580e8498，2026年11月8日00:55:19北京时间。这些是补充项目文档，不冒充新的窗口候选或独立测试。README把流程分为带注释.mpd研究、子模型／机构拆分、运动规划、转换同标签.glb、生成Blender脚本。样例标注Sonnet 5.5和Opus 5.5，保留42043缩小范围；Gallery另有42000转向／差速／V8、42083独立机构等。

验证文档区分计划运动、Blender实现与保存动画：变换对照、混合姿态、重开文件、采样间隙和人工视觉复核不能互相替代。--require-reviewed可包含明确defer，并不发现漏掉的机构；间隙采样不证明连续无碰撞、包含关系或原本接触处没有恶化。工具实现声明的刚体运动学，不保证力、摩擦、齿隙、通用闭环／接触求解或柔性材料物理。10265 v2示例的门、后部车高调节、换挡及增压器未实现；发现接触点的修正不追认旧rig正确。

项目要求Python3.12+；README的Linux x86_64及Windows/WSL2路径为WIP未测。候选称没有物理引擎与软管问题，只按其转述保留，以上补充文档给出更精确边界。不把渲染流畅当真实机械可行，也不把原作者的成功样例当任意模型全自动成功。未安装依赖、运行目标、观看视频或重做验证；未声称使用REA。

候选封存0赞、205浏览、0转发；传播弱不等于项目无价值，文档核对不等于复现。
标签解析提交日期早于候选；仅阅读公开文本，未执行项目测试。

## 来源

- [Xiao Tan的LDraw Mecha介绍与42043缩小范围，2026-11-08 05:17北京时间](https://x.com/i/status/2119177320703357172)
- [补充：antelocnova的Show HN项目说明，2026-11-07 03:41:20北京时间，早于本窗](https://news.ycombinator.com/item?id=50397325)
- [补充固定README：v0.5.0对应11月8日00:55:19北京时间提交](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/README.md)
- [同提交Gallery：模型与动画样例目录，非本合集观看记录](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/GALLERY.md)
- [同提交验证文档：运动学、覆盖与物理边界](https://github.com/anteloc/ldraw-mecha/blob/c09ad90caf4f4cba00b1542eb622de8e580e8498/docs/validation.md)

[English](en/ldraw-mecha-semantic-parts-blender-motion.md) | [返回目录](../README.zh-CN.md)
