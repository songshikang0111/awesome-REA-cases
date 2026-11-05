# Apple Neural Engine：Claude 辅助私有 API 研究与600M模型训练的转述

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-05
阶段：待验证

10月18日16:27（北京时间），@_vmlops（Vaishnavi）转述有人使用Claude逆向Apple Neural Engine，借助私有API而非CoreML，在该硬件上训练600M参数模型。具体用途是利用原本不受官方路径支持的训练能力，不是破解模型权重。

较早候选没有具名原开发者。2026年11月5日20:08:11（北京时间）的新候选将Claude辅助私有API研究和网络训练归于@originalmaderix，补上可识别的开发者线索，但没有再次给出600M或训练验证，不把两次转述当独立复现。芯片型号、系统版本、训练步骤、精度、耗时或可核验仓库仍未取得，600M仅为较早转述参数规模。

不能确认训练是否全在神经引擎执行、是否包含反向传播或可迁移到所有Apple设备；也不能从感叹推断完整训练成功。较早原帖身份与正文已补取，未获得独立训练验证，未确认REA。

10月18日候选快照15赞、612浏览、1转发；600M为第三方说法，不是本合集实测。
11月5日新候选封存0赞、12浏览、0转发；补充作者线索，未补训练测试。

## 来源

- [Vaishnavi 的 ANE／Claude 训练转述](https://x.com/i/status/2111735919556624880)
- [新候选：归因originalmaderix的ANE私有API／Claude研究，2026-11-05 20:08:11](https://x.com/i/status/2118314432963215869)

[English](en/apple-neural-engine-claude-training-report.md) | [返回目录](../README.zh-CN.md)
