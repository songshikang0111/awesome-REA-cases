# HookLab：REA研究Creator Hooks，Claude重建YouTube标题与异常视频库

分类：应用与客户端 · REA
记录日期：2026-11-03
阶段：进行中

2026年11月3日00:29（北京时间），Samin Yasar（@SaminXD）报告停止支付每年360美元的YouTube工具费用，以REA研究后用AI编程Agent重建HookLab。它面向视频创作者：按真实异常高表现视频生成分角度标题，搜索超过频道平均表现的视频，轮询新上传并用Claude打标签，提供CLI与REST API。价格与停订是作者自述，不是净运行成本。

补查公开Samin12/hooklab固定提交1e5fcb584c98b0b3bfe44438ee4410414b91990d的README、HOW-IT-WAS-BUILT与app/package.json。该提交时间为10月19日06:00:22北京时间，早于候选窗口，作为既有实现和方法背景，而非11月3日新提交。方法文档点名原工具Creator Hooks：作者在独立浏览器profile登录，让REA经DevTools读取DOM、可访问性树、网络元数据、存储键和加载脚本，点击屏幕补齐懒加载后导出脚本；分析压缩包、48个click-trigger标签及无source map的客户端，再录制一次真实标题聊天的请求与流式响应。随后由Claude Code做基础层，四个worker分别构建不同界面，再加数据CLI／API和轮询流水线。

文档称My Channel的个人视频／近期均值倍数在所比较视频上重现原数值，但没有比较样本数、原输出或全功能差分记录，不能升级成恢复服务端算法或完整等价。项目自称不含原工具代码、资产或数据；本合集没有审计这一声明或净室隔离。

README要求Node.js 24，Next.js 16与本地SQLite；新装库为空，须自行加频道。聊天／标签需Anthropic API或已登录Claude Code，轮询用YouTube RSS，发现和部分元数据可选ScrapeCreators；自托管不等于离线或零费用。缩略图搜索只用标题文本，没有图像嵌入；billing只是本地额度账本，不会收费。仅读取公开文档和manifest，未安装依赖、运行目标、登录服务或重跑比较。

候选快照20赞、826浏览、2转发；每年360美元为作者原订阅费用，不代表AI与数据服务免费。

## 来源

- [Samin Yasar的HookLab／REA报告，2026-11-03](https://x.com/i/status/2117292948488400976)
- [补充固定README：已有实现与依赖，2026-10-19，早于窗口](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/README.md)
- [补充固定方法文档：Creator Hooks研究与重建，早于窗口](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/docs/HOW-IT-WAS-BUILT.md)
- [补充固定app/package.json：声明依赖，未安装](https://github.com/Samin12/hooklab/blob/1e5fcb584c98b0b3bfe44438ee4410414b91990d/app/package.json)

[English](en/hooklab-rea-youtube-outlier-tool-rebuild.md) | [返回目录](../README.zh-CN.md)
