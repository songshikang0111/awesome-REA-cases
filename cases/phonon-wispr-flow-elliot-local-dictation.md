# Phonon：Elliot用DeepSeek与Opus重建Wispr Flow式本地听写

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-06
阶段：进行中

2026年11月6日00:53:02（北京时间），Elliot Arledge（@elliotarledge）称逆向Wispr Flow，再用DeepSeek微调LFM3-1.7B、用Claude Opus 5.5 [xhigh]构建Phonon，以本地语音输入替代付费听写流程。Parakeet识别、refiner整理文字，两者在讲话时流式工作；按目标应用选择Discord口语、Slack/邮件正式文体、Claude Code提示词模式，支持导入个人词典。这与此前Vraj的Wispr替代品是不同作者、不同具名项目，不能因目标相同而合并。

作者报告M4 Max松键到文字65ms，对同片段Wispr Flow约520ms；六分钟讲话结束约四分之一秒。Rust后端、原生Metal融合解码核和dflash2推测解码器来自其说明，称在本地四张RTX Pro 6000上训练drafter。训练为约77k公共音频转录与合成听写，由DeepSeek v4.1 flash 1017按四种文体重写，未用个人听写；以Claude Opus盲评一小时讲座，Phonon获90次偏好、Wispr 23次。这不是人类盲测、标准准确率或本合集复现，也不证明对所有口音与应用相等。

补读公开仓库固定提交2e9a5b724845b7b5881701f06c08d00deccc3e5f的README与许可，提交于11月6日03:24:41北京时间，属于补充项目材料、不是另一个候选。文档写76,960条数据、macOS 14+与Apple Silicon，首次下载约4.9GB模型及Python依赖；后续听写本地运行，但默认每日查GitHub更新，可关闭。原生引擎不能运行时回退MLX；文档另报40次真实听写的引擎内中位数从215ms降到30ms，口径不同，不拿来替换65ms端到端自述。Windows仍beta、未签名，使用ONNX与Gemma/llama.cpp CPU路径，不能把Mac的LFM3/Metal性能套过去。

README说明本地历史与屏幕上下文默认关闭，需麦克风、辅助功能和输入监控权限，启用屏幕上下文另需录屏权限。源码GPL-3.0；权重保留各自许可，文档称Parakeet为CC-BY-4.0、LFM衍生refiner商业使用受年收入低于1000万美元条件限制，不能概括为所有组件无条件开源商用。未审计全部源代码、网络行为或模型训练，未安装、运行或重测；逆向归因仍来自作者，公开实现不证明恢复了Wispr内部源码。未提REA。

候选封存722赞、21201浏览、43转发；实时补取上涨不替换快照。性能、90对23偏好及训练资源均为作者或项目自报，非独立评测。

## 来源

- [Elliot的Phonon／Wispr Flow研究与自测报告，2026-11-06 00:53:02北京时间](https://x.com/i/status/2118386115170496855)
- [补充Phonon固定README，提交2026-11-06 03:24:41北京时间](https://github.com/Infatoshi/phonon/blob/2e9a5b724845b7b5881701f06c08d00deccc3e5f/README.md)
- [同提交源码GPL-3.0许可；权重限制另见README](https://github.com/Infatoshi/phonon/blob/2e9a5b724845b7b5881701f06c08d00deccc3e5f/LICENSE)

[English](en/phonon-wispr-flow-elliot-local-dictation.md) | [返回目录](../README.zh-CN.md)
