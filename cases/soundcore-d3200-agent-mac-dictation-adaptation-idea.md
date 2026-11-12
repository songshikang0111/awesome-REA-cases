# Soundcore D3200到Mac输入法：让Agent改造实时取流客户端的idea

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-12
阶段：进行中

2026年11月12日09:39:52（北京时间），AI产品黄叔（@PMbackttfuture）介绍用安克录音豆替代Typeless一类语音输入流程，称自己使用Mac上的微信语音输入法，并建议让Agent稍改tacshi/Soundcore、或用ASR自建输入法。作者一面说方案已破解、零费用零延时，一面说识别后粘贴到当前光标的最后一段尚缺，因此不写成已交付的全链路输入法。

09:34:11另一候选介绍Soundcore Manager为soundcore Work D3200的Flutter本地客户端，脱离飞书管理录音。补读tacshi/Soundcore固定提交bfd764a2aad55aca103a86e7d6ca2c814d3f7f9c的README；提交日期为2026年9月11日19:20北京时间，早于本窗口，仅用于核基础能力。文档列Android／iOS／macOS、BLE配对与实时音频、录音管理、SoftAP导出、Apple设备端或Soniox转写；Apple设备端说明限定iOS26以上及设备／语言支持，不能据此声称Mac也能本地调用同一接口。Soniox批量路径会上传录音，故本地管理不等于全流程离线或零费用。

这是上游协议客户端上的Agent辅助改造方向，不证明上游协议本身由AI逆向。它与基线BeanScribe同用D3200但实现和用途不同：这里是Flutter客户端到Mac当前光标输入的设想，BeanScribe是飞书H5／Python及文档链路，不合并成果。作者称仓库缺许可证，但本合集只核README，没有核完整许可树；不认可其自己用就没问题的法律推断。附视频未审，无改造提交、端到端测试或延迟测量，保持进行中。本合集未构建、连接设备或调用识别服务。

封存主帖13赞、1293浏览、1转发、4回复；功能介绍帖3赞、46浏览、0转发。237星是作者当日声称，未独立核星数；零费用、零延迟无测量。

## 来源

- [AI产品黄叔的Agent改造与Mac输入法方案，2026-11-12 09:39:52北京时间](https://x.com/i/status/2120693023420112940)
- [同窗Soundcore Manager D3200功能介绍，2026-11-12 09:34:11北京时间](https://x.com/i/status/2120691593128640855)
- [补充固定README：2026-09-11 19:20北京时间提交，早于候选；11月12日静态查阅](https://github.com/tacshi/Soundcore/blob/bfd764a2aad55aca103a86e7d6ca2c814d3f7f9c/README.md)

[English](en/soundcore-d3200-agent-mac-dictation-adaptation-idea.md) | [返回目录](../README.zh-CN.md)
