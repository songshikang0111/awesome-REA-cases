# designlang：从既有网页提取设计Token，供Agent与多端重建使用

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-05
阶段：相关项目

2026年11月5日10:20:40（北京时间），一帖推荐design-extract（designlang），称通过npx designlang <url>研究既有网站的设计系统，并通过MCP把结果交给Claude Code、Cursor、Windsurf。具体对象是可渲染网页的颜色、排版、阴影、组件及交互状态，面向竞品参考、跨端重建和设计漂移检查，不是反编译网页后端。

转述称基于Node.js20+和Playwright，捕获四个响应式断点、hover/focus属性变化、多页一致性，输出DTCG Token、Tailwind v4、shadcn/ui、SwiftUI、Compose、Flutter以及Figma变量，附WCAG对比度修复建议与sync。这里只保留这些为来源宣称；没有具名网站、导出物、运行日志、许可正文或质量对照，未直接核验仓库。

完整抽离任意设计哲学、永不漂移等为推广措辞，不是覆盖或正确率证明；约4.5k星是11月5日帖子口径。没有依据认定模型自动调用全部功能或产物可直接投产，REA未提。按相关工具项目收录；未运行npx、安装依赖或抓取目标站点。

候选封存2赞、120浏览、0转发；约4.5k星、四断点及平台清单均为转述，未复核。

## 来源

- [候选：design-extract/designlang设计提取与MCP转述，2026-11-05 10:20:40](https://x.com/i/status/2118166578521084221)

[English](en/designlang-website-design-token-agent-extraction.md) | [返回目录](../README.zh-CN.md)
