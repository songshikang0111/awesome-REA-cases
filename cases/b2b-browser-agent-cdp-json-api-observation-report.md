# B2B门户取数：SaasNext称浏览器Agent经CDP读取原始JSON

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-10-30
阶段：待验证

2026年10月30日15:31:52（北京时间），SaasNext（@Saasnext_db）比较无头浏览器Agent与直接后台API逆向，称自己的Agent登录供应商门户后不抓渲染HTML表格，而监听Chrome DevTools Protocol的Network.responseReceived事件，直接读取原始JSON响应。具体用途是从已登录、可观察的业务界面恢复结构化数据输入，减少对像素识别的依赖；不是证明已恢复后台源码或绕过权限。

作者报告640ms的p95响应时间与零OCR幻觉，但没有计时起止、样本量、网络/硬件环境、门户身份、Agent/模型、对照基线、代码或日志。完全不用OCR能避免该步骤的误识别，不代表JSON完整、业务映射正确或所有Agent推理无幻觉。帖子未明确哪个环节由模型进行，不补填模型能力或REA使用。本合集仅核对原帖，未登录门户、截取流量或运行Agent；保留为未验证的Agent接口观察/重建工作流报告。

候选快照0赞、2浏览、0转发；640ms与零OCR幻觉未独立计量，模型分工不明。

## 来源

- [SaasNext的CDP取数与640ms p95自述，2026-10-30](https://x.com/i/status/2116070565358305716)

[English](en/b2b-browser-agent-cdp-json-api-observation-report.md) | [返回目录](../README.zh-CN.md)
