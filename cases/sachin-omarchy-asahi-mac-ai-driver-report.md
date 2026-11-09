# Mac上的Omarchy：AI硬件适配与Asahi依赖的相互冲突转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-09
阶段：待验证

2026年11月8日18:06:46（北京时间），Sachin（@sachintwtss）称Omarchy借Asahi逆向与AI agents在Mac实现Touch ID、M3 GPU和deep sleep，并说Asahi因禁止AI代码不接收相关上游修改。他承认clean-room法律顾虑，但未提供驱动或AI分工。AI贡献政策不是代码许可证，不能据其评论断言全部驱动来源或法律状态。

11月9日03:06:37，@me_deepu转述DHH团队用Agent推进这些功能，增加DisplayPort over USB-C与MacBook Neo，并解释洁净室知识来源顾虑：不许泄露Apple材料，模型可能见过人没见过的材料，Agent还会掩盖答案来源。旧补取只确认评论者和措辞，未读DHH原声明或政策全文，非官方支持或拒收结论。

11月9日16:44:32，Miklos（@MiklosDenmark）在另一段相关讨论中明确说Omarchy不使用Asahi，质疑AI如何污染来源以及为什么把该例称为洁净室，称只是普通逆向。补取确认署名、文字及回复关系，但没有代码或架构证据裁定双方。新反驳使此前Asahi基础上的表述更应保持归因；不能只凭另一条评论把争议改成已证实不依赖，也不能继续把依赖关系写成事实。

始终未取得对应Omarchy/Asahi提交、准确机型、内核版本、Touch ID认证、M3渲染、USB-C显示或休眠唤醒日志。保留原帖MacBook Neo等名称，不据其推断硬件。硬件支持、AI分工、上游拒收和依赖全是尚有争议的二手说法，不重新将Asahi既有人工研究归功AI。REA未提及；本合集未安装发行版、执行补丁或连接Mac，状态仍未核验。

较早候选2赞、257浏览、0转发；硬件和不上游说法未获官方确认。
11月9日03:06候选0赞、17浏览、0转发，新增功能与政策关系仍为二手说明。
11月9日16:44候选1赞、118浏览、0转发；反驳亦无代码证明，不裁定依赖或洁净室法律状态。

## 来源

- [Sachin的Omarchy／Asahi与AI agents转述，2026-11-08 18:06:46北京时间](https://x.com/i/status/2119371038069060078)
- [me_deepu转述DHH团队的USB-C显示、MacBook Neo与洁净室政策，2026-11-09](https://x.com/i/status/2119506897766359542)
- [Miklos反驳Asahi依赖与洁净室前提，2026-11-09 16:44:32北京时间](https://x.com/i/status/2119712731758571757)

[English](en/sachin-omarchy-asahi-mac-ai-driver-report.md) | [返回目录](../README.zh-CN.md)
