# Facebook照片模型：Alex Choi让Claude Code研究Android应用

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-06
阶段：待验证

2026年11月6日00:54:18（北京时间），Alex Choi（@AlexChhk）称手机显示Facebook凌晨04:32在其睡觉时读取照片，于是让Claude Code反编译Android v585.0.0.47.54，调查应用对相册做什么。作者报告发现按aesthetics与shareworthiness评分、识别宠物和场景的AI模型，并声称会给相册每张照片打分。

补取确认作者和附图存在，但未取得APK哈希、模型文件、反编译调用链、权限条件、原始访问日志或网络抓包。即便模型静态存在，也不能推出每张照片都已扫描、在04:32触发的正是该模型、照片被上传或用途为广告；时间、发现和因果均保持作者报告。作者此前研究Instagram的已安装应用检测是不同软件与研究问题，不把两者合成已证明Meta统一监控机制。未提REA，本合集未读取私人相册、连接设备或运行应用。

封存13赞、455浏览、1转发；模型及凌晨读取均为作者自述，未独立验证。

## 来源

- [Alex Choi的Facebook／Claude Code照片模型调查，2026-11-06](https://x.com/i/status/2118386433727852901)

[English](en/facebook-android-claude-photo-model-investigation.md) | [返回目录](../README.zh-CN.md)
