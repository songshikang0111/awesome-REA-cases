# HyperFrames RAV：Stripe重建自述与20片竞争工具比较

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-07
阶段：待验证

2026年11月5日02:41:49（北京时间），Miguel Ángel（@Miguel07Code）说受morluto的REA启发，与HyperFrames发布RAV，即/reverse-any-video，并给出技能更新命令，称完整1-shot重建Stripe发布视频。它是参考视频结构与表现的重建，不是软件二进制分析。开源为作者说法；未取得可确认源码位置、许可、技能正文、原始输入、提示、生成记录或逐镜对照，视频未观看。1-shot不等于无准备、编辑或重试，也不证明找回原提示词、配乐与资产。

11月7日03:41:51，Miao Yang（@WaterrrMiao）以our reverse-any-video对REA-VIDEO报告20片比较，涵盖UGC、口播及动态图形。实验一以人工标切点为参照，按其先后顺序，RAV／REA-VIDEO发现108/108对59/108切点，precision96%对89%，耗时81秒对1595秒，称约20倍；还说后者在八例中三例把实拍当AI。实验二称同模型、同keys、隔离容器做1:1重做，SSIM0.96对0.78，同时承认REA-VIDEO重做略快且便宜。作者认为复杂口播、B-roll、重编辑与发布动效更显己方优势，简单UGC两者都好。

补取确认比较者署名，但没有20片清单、每片标签、软件版本、配置、模型名称、绝对重做费用／时间、SSIM对齐及聚合方法或可重跑记录，也未独立确认与先前HyperFrames版本的连续性；按同名技能的后续报告追加，不当独立基准。分析速度与成片速度是两个实验，不能混成全面更快。切点precision、SSIM与REA-VIDEO自身按时长加权的制作来源判定准确率不是同一指标。

REA仅为灵感来源，未确认执行；与HyperFrames editor小Lin说／Vox模板及REA-VIDEO保持区分。未安装技能、下载原片、观看比较或运行重建，保持unverified。

11月5日封存11赞、627浏览、2转发；开源与1-shot是作者说法，不是源码或成片核验。
11月7日较早候选2赞、42浏览、0转发；20片、108切点、precision、时间与SSIM均为竞争方报告，不是本合集复测。
11月7日10:12:50，James Russo（@Rames_Jusso）建议用HyperFrames逆向并混剪视频，称己方评测对REA-VIDEO每个维度都胜出。补取确认署名，但未获得该帖对应的版本、样本、指标表或原始结果；不能把它当成新独立实验。较早详细比较明确承认REA-VIDEO成片略快且便宜，因此全面胜出的宣传不应覆盖该边界。候选封存6赞、390浏览、0转发。

## 来源

- [Miguel Ángel的HyperFrames RAV发布与Stripe示例，2026-11-05](https://x.com/i/status/2118051103057101245)
- [Miao Yang的reverse-any-video对REA-VIDEO自测，2026-11-07 03:41:51北京时间](https://x.com/i/status/2118790987875221905)
- [James Russo的全面胜出宣称，2026-11-07 10:12:50北京时间](https://x.com/i/status/2118889384162525495)

[English](en/hyperframes-rav-stripe-video-reconstruction.md) | [返回目录](../README.zh-CN.md)
