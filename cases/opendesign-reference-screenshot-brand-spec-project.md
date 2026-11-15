# OpenDesign：从参考截图提炼品牌规范，再交给编码Agent重建界面的工作台

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：相关项目

2026年11月15日09:46:09（北京时间），AIWare（@aiwaremax）介绍nexu-io的OpenDesign。背景是编码Agent分别生成落地页、后台、PPT和视频时，字号、圆角与配色容易失去一致性；与本合集相关的具体功能是从已有品牌的参考截图研究视觉规则，再形成可复用规范，而非反编译Claude Design或恢复其源码。

补读公开仓库固定提交59e4f2ae85de7e7318a5e6bdcf3a34584c4b7582的README，提交时间为2026年11月13日09:15:18 UTC，早于本窗口，仅作方法补证。文档描述提交截图或URL，由Agent整理可复用DESIGN.md，再把规范与插件、模板结合生成HTML/CSS产物，并交给Claude Code、Codex或Cursor继续开发；stdio MCP可以读取项目中的tokens CSS、JSX与HTML等当前文件。这支持品牌规范提炼及后续重建的项目定位，不证明对任意截图都能精确恢复设计系统、交互或后端。

候选列151套品牌系统、277个官方插件、183个参考示例和26种Agent CLI。所读README也给出这些目录规模，但说明旧设计包可能只有DESIGN.md，新包才可能附manifest、tokens.css、组件、资产与来源记录；不能把每套都描述为完整tokens实现。未遍历目录核数，也未实测全部适配器。107102个GitHub星是候选的宣传快照，没有独立核实。

README称Apache-2.0，第三方素材与品牌权利仍须另行确认。Local-first不等于离线或绝不外发：文档明确云端模型／OpenDesign Cloud请求会发送到相应服务，安全与可靠性遥测始终开启，产品分析及会话回放则征求同意。未安装工具、连接MCP、上传截图、运行提取或比对输出，按具体AI辅助视觉规则研究的相关项目收录；REA未提及，准确性与可用性均未独立验证。

封存候选4赞、475浏览、0转发、13回复；107102星为帖子声称的快照。
151套系统、277插件、183示例与26种CLI是项目／介绍者的目录口径，不是本合集测得的准确率、完整覆盖或节省工时。

## 来源

- [AIWare介绍OpenDesign参考截图品牌提炼与编码Agent工作流，2026-11-15 09:46:09北京时间](https://x.com/i/status/2121781771750854878)
- [窗口前固定README：截图／URL到DESIGN.md、包结构及数据外发说明，提交2026-11-13 09:15:18 UTC](https://github.com/nexu-io/open-design/blob/59e4f2ae85de7e7318a5e6bdcf3a34584c4b7582/README.md)

[English](en/opendesign-reference-screenshot-brand-spec-project.md) | [返回目录](../README.zh-CN.md)
