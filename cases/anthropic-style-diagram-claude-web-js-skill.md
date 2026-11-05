# Anthropic风格图表Skill：耳朵观察Claude绘图时的JS加载来重建规范

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-05
阶段：进行中

2026年11月5日14:47:36（北京时间），耳朵（@RookieRicardoR）回顾逆向网页版Claude design：先让Claude画图，观察绘SVG时额外加载的JS，再问Claude需要加载什么，以定位规范、组件和尺寸约束，最终做成anthropic-style-diagram Skill。目标是把Claude式技术图表视觉规范带到可复用本地工作流，不是训练模型或破解账号。

补读公开erduo-skills固定提交1fb6ec5df76c01dc43fb71631b8ae6121b9251df的README及SKILL.md；提交日期为7月26日00:44:44北京时间，早于本窗口，仅作产物文档证据。Skill让Agent写几何与语义类名，render.mjs注入配色、主题和字体，审计文字溢出、节点重叠、连线穿越，裁切并导出PNG与独立SVG，支持亮暗主题。文档要求Playwright，几何审计通过后仍须人工查看箭头、反馈回路、文字与分类颜色，明确版式通过不保证语义正确。

这确认有公开工作流文档，不证明其与Claude官方内部Skill逐字一致、原始提示词已泄露或所有图均准确。没有观察JS的原始记录、官方对照或运行测试；README称MIT，未做全面许可审计。本合集未安装依赖或执行渲染，REA未提。

候选封存6赞、480浏览、0转发；补取确认作者，较高实时计数不替换。

## 来源

- [候选及署名补查：耳朵的Claude网页JS／SVG研究回顾，2026-11-05 14:47:36](https://x.com/i/status/2118233755966218710)
- [补充项目README：固定7月26日提交，非本窗成果日期](https://github.com/rookie-ricardo/erduo-skills/blob/1fb6ec5df76c01dc43fb71631b8ae6121b9251df/README.md)
- [补充Skill：绘图契约、几何审计与语义复核，固定同一提交](https://github.com/rookie-ricardo/erduo-skills/blob/1fb6ec5df76c01dc43fb71631b8ae6121b9251df/skills/anthropic-style-diagram/SKILL.md)

[English](en/anthropic-style-diagram-claude-web-js-skill.md) | [返回目录](../README.zh-CN.md)
