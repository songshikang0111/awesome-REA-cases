# reanimate：Claude Code逐帧记录、重建与比较网页动画的公开skill

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-31
阶段：分析测试

2026年10月31日10:02:00（北京时间），Agent Skills Hub（@agentskillshub）在技能盘点中介绍NiazMorshed2007/reanimate，称可让Claude Code逐帧逆向任意动画并验证一致。补读固定提交522a353be364828ef43e1440faf5c1077edccbc1的README，提交时间为10月30日10:31:21北京时间，早于候选；文档和项目测量不能把“任意”“一模一样”推广为保证。

项目目标是克服只凭截图重建一次就结束、看不到运动误差的问题。它从网站、录屏、mp4、gif或Lottie录取参考，在固定视口与帧率下记录视频、逐帧元素位置和CSS／Web Animations信息；形成每元素每属性的时长、起终值、easing和stagger规格，再用目标项目已有CSS、Framer Motion、GSAP或three.js实现，同样录制副本，比较时序、曲线与像素。通常称2到5轮，五轮仍不匹配的列出原因，而非一律报成功。

默认匹配运动，允许时序误差80ms；精确外观模式另要求平均像素差不超过2%。公开样例涉及Stripe卡片、WorkOS、Clerk、Liveblocks、Resend等，项目称多数耗时30到80分钟；例如Stripe卡片静止像素差0.03%、倾斜差0.4px，属于项目自测，不是本合集重跑。Canvas／WebGL路径记录GPU调用、shader、uniform与场景图，并用虚拟时钟和随机种子减小捕获变化；这也可能读取原站素材与代码，不能概括成绝不复制源码的净室保证。

文档要求Bun1.1以上，macOS／Linux环境，Windows未测；只报告测试Claude Code，其他Agent兼容未证实。登录页、YouTube和Loom不能直接录取，需用户提供录屏；worker自己的时钟仍走实时时间，不能复用随机生成器时按模糊分布比较粒子，而非逐点相同；Linux硬件GPU路径未测。字体、图像和代码的权利仍属原作者。未安装依赖、打开目标网站、抓素材或运行skill，不宣称普遍等价、安全或授权无风险；REA未提及。

候选快照0赞、50浏览、0转发；盘点称101星，未作为功能证明。
80ms、2%、0.03%、0.4px及30到80分钟均为项目文档口径，未独立复测。

## 来源

- [Agent Skills Hub技能盘点中的reanimate，2026-10-31](https://x.com/i/status/2116349940666703976)
- [补充：reanimate固定README，样例测量、比较阈值与限制，2026-10-30](https://github.com/NiazMorshed2007/reanimate/blob/522a353be364828ef43e1440faf5c1077edccbc1/README.md)

[English](en/reanimate-claude-animation-record-rebuild-compare.md) | [返回目录](../README.zh-CN.md)
