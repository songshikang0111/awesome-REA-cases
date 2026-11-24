# echo-dot-assist：Claude参与替换Alexa，保留旧Echo的麦克风与唤醒

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-24
阶段：进行中

2026年11月24日08:09:25（北京时间），Michael_AI_Hu发布《闲置Echo改接家里的助手》，介绍Julian Imhof的echo-dot-assist。补读文章全文，并读取项目09:32:18版本7489169的README；该版本在本轮窗口内，属于补充文档而非另一候选。目标是利用闲置Amazon Echo的远场麦克风、原音频处理与唤醒能力，以小守护进程hassmic替换Alexa客户端，保留Fire OS，让Home Assistant把它发现为ESPHome语音卫星。

README明确代码、笔记与文档由作者和Claude对话写成；不等于Claude独自逆向所有固件。取得设备控制权的MediaTek利用、kaeru与TWRP移植归R0rt1z2，项目要求按型号手工解锁，不把这些前人成果归给AI。文档列本地多设备应答协商、定时器、播报、追问、局域网Drop In、Music Assistant多房间播放、蓝牙及按键／灯环自动化；Wyoming模式只有语音、唤醒、按键和音乐等子集。Echo Show屏幕叠字、Wi-Fi运动感知仍实验性，声音检测较不可靠。功能均为项目说明，非本合集实测。

支持表列Dot 2／3、Echo 2、两代Show 5／8和Input，Dot 5仅手工安装；不能据外观推断所有代际均支持。2019—2020的Dot 3 C78MP8及带时钟36EBT3明确不支持。作者每型号只试一台，代码未经审计；解锁与system分区写入会清空设备并可能变砖，部分设备要拆焊和指定固件。主解锁路径要求实体Linux直连USB，Windows只接已解锁设备。文章还指出Windows全新设备完整路径尚无走通报告。

不联系Amazon是防火墙设计目标，不是已证明零外联：文章提醒原守护进程可能做DNS，回复／音乐地址由Home Assistant或Music Assistant给出；README承认防火墙或更新错误可使设备联外网或在局域网暴露，加入Home Assistant之前同网其他人可连接。已读公开README，未读全部源码或设备页，未解锁、刷写、运行安装器、连接硬件或核验隔离。项目原创代码MIT不授权Amazon固件、库与唤醒模型。与既有LibreEcho不同仓库，不合并，REA未提。

候选封存0赞、96浏览、0转发、0回复；每型号一台为项目测试口径，不是独立复现或大规模可靠性验证。

## 来源

- [Michael_AI_Hu的echo-dot-assist长文，2026-11-24 08:09:25北京时间](https://x.com/i/status/2125018915772477502)
- [补充第一方README：Claude归因、单台测试、支持范围与风险；7489169，2026-11-24 09:32:18北京时间](https://github.com/Gamer92000/echo-dot-assist/blob/7489169851ac0e196ac0a8647cef2b80ca1f716b/README.md)

[English](en/echo-dot-assist-claude-hassmic-home-assistant.md) | [返回目录](../README.zh-CN.md)
