# OKOK Libre：REA与GLM研究体脂秤APK，重建离线Android客户端

分类：应用与客户端 · REA
记录日期：2026-10-31
阶段：进行中

2026年10月31日19:13:19（北京时间），JYunth（@j_yunth）说在Zepto买的Ant Esports体脂秤只能配合广告多、加载差的OKOK International。他称用REA加GLM5.3研究约50MB APK，提取公式和API，重建OKOK Libre，由Opus5.5制作UI，并指控原应用向中国服务器上传体重。外传与“每个公式／相同数学”都只是作者说法，本合集未检查原APK、抓包或对照公式。

补读同作者公开仓库JYunth/okok-libre在093a337a86025c532e0afd21e86fd856c8c5c00a的完整README、主AndroidManifest和CI定义。提交日期为10月31日18:44:40北京时间，早于候选，注明Claude Opus5.5共同署名。README要求Android8.0及以上、Bluetooth LE；支持classic、OKOKCloud、OKOKCloudV4，明确部分其他设备家族未实现。秤可能只报体重、提供阻抗或自行计算体成分，不能称所有OKOK秤及指标都兼容。文档列多用户、本地趋势、备份与表格导出；截图是虚构演示家庭，不是真实健康数据。

固定主Manifest未声明INTERNET或广告ID权限，并关闭备份；这是静态文件检查，不是对最终APK合并权限、网络行为或安全性的运行审计。README提醒手工备份未加密，体成分只是估计而非医疗建议。GPL-3.0公开实现与测试源码可查，CI定义包含单元测试及debug／release构建，但未在此运行；不把工作流文件当测试通过证明。本合集未安装依赖、下载APK、连接秤或复现，保留进行中、协议范围与公式未核验边界。

候选快照0赞、14浏览、0转发；50MB为作者口径，不以热度证明功能。
Android8.0+、三种协议为固定文档范围；未实测兼容或体成分准确性。

## 来源

- [JYunth的REA／GLM／Opus体脂秤客户端报告，2026-10-31](https://x.com/i/status/2116488683188887716)
- [补充：固定README的协议兼容与隐私边界，2026-10-31](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/README.md)
- [补充：固定主AndroidManifest静态权限，2026-10-31](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/app/app/src/main/AndroidManifest.xml)
- [补充：固定CI定义而非通过证明，2026-10-31](https://github.com/JYunth/okok-libre/blob/093a337a86025c532e0afd21e86fd856c8c5c00a/.github/workflows/ci.yml)

[English](en/okok-libre-rea-glm-scale-android.md) | [返回目录](../README.zh-CN.md)
