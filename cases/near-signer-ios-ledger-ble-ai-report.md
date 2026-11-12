# NEAR Signer：AI协作开发的iPhone Ledger协议兼容端，实机仍待核

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-12
阶段：进行中

2026年11月12日13:01:43（北京时间），莫信（@musinoot）介绍near/near-signer-ios：把iPhone作为NEAR交易与消息签名设备，通过Ledger Nano X的蓝牙接口让既有near-connect和near-cli-rs连接，也支持二维码传递请求和签名。文章转述Vlad Frolov说由Ivan Frolov及其agents编写，并称Claude审查代码；这是具体协议兼容实现，不证明AI反编译Ledger固件或恢复原源码，REA未提及。补取同一原帖获得完整后半段，不能只据前半宣传声称已实机验证。

补读固定提交c779108b128a47f9753edbd54131b0de6a352149的README，提交于11月12日01:16:14，早于候选；它确认NEAR Ledger APDU与Nano X BLE framing，列near-cli-rs 0.25及以上和Chrome／Edge的near-connect，要求App保持前台。iOS不能充当USB Ledger，Safari／Firefox无Web Bluetooth；My Ledger设备管理需要固件详情与真机验证，不能工作。文档列二维码通道，未知动作或无法完整解析的请求拒签，用户看完字段后批准并用Face ID或密码解锁。

安全边界不能写成真Ledger等价：Secure Enclave不能存NEAR所需ed25519私钥，项目改用P-256钥匙加密保存，签名时解密到应用进程，文档称不备份或同步iCloud。公开README的验证节自报Linux上128个Swift测试、14个Python端到端测试通过，near-connect在模拟BLE链路完成握手与签名，near-cli-rs 0.30.1与模拟器输出匹配，二维码编解码有17个Node和20个Rust测试；丢帧模拟包括30%重排丢失及300KB部署20%丢失，不是iPhone摄像头实测。

同一验证节明确因没有Mac或iPhone，未核真实Xcode构建、界面、与macOS／Linux／Windows配对的蓝牙无线行为、手机扫码速度或真实摄像头回读；手写框架替身的类型检查不能替代Apple SDK构建。文档另列Claude PR审查流程，不等于第三方安全审计。候选称需自行Xcode 26构建、iOS 17以上且App未上架，二维码工具0.1.0不是手机App发布版。本合集未构建、运行测试、连接钱包或签交易，保留进行中与项目自测归因。

候选封存0赞、313浏览、0转发；1星为作者中午读取的传播快照，未独立核热度。
所有测试数字为固定README的项目报告；未运行，不证明真实设备或资金安全。

## 来源

- [莫信的NEAR Signer项目整理，2026-11-12 13:01:43北京时间；补取同帖完整文字](https://x.com/i/status/2120743823085281609)
- [补充固定NEAR Signer README，2026-11-12 01:16:14北京时间提交，早于候选；协议、安全与验证范围](https://github.com/near/near-signer-ios/blob/c779108b128a47f9753edbd54131b0de6a352149/README.md)

[English](en/near-signer-ios-ledger-ble-ai-report.md) | [返回目录](../README.zh-CN.md)
