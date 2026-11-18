# MapSleuth：Robbie用两台DGX Spark的本地AI研究ECU标定表

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-19
阶段：进行中

2026年11月19日01:08:07（北京时间），Robbie Searles（@rsearles35）介绍正在制作的MapSleuth。ECU是汽车电子控制单元，标定表保存控制行为所需的参数映射；项目目标是在ECU固件里找到并解码这些表，使用两台DGX Spark上的本地AI。没有给出车型、ECU型号、固件版本、具体表或AI模型，不据此声称已安全完成车辆调校。

作者称刚把模型后端从vLLM迁到TensorFold，输出速度从约40升为57 tok/s，首token时间从约1.25秒降至0.18秒。这些是其环境下的推理性能自述，不是地图识别准确率、解码完整率或车辆性能，也没有公开测试条件或重复运行数据。

补取原帖确认署名、完整文字与日期；未审图片、源码、固件样本或日志，未运行模型或接触车辆。保留进行中项目，REA未提及，不提供写入ECU、绕过车辆安全限制或上路调校指令。

候选封存3赞、55浏览、0转发、2回复；速度与首token值为作者自述，没有ECU识别基准。

## 来源

- [Robbie的MapSleuth与本地推理迁移报告，2026-11-19 01:08:07北京时间](https://x.com/i/status/2123100953595240836)

[English](en/mapsleuth-local-ai-ecu-calibration-map-research.md) | [返回目录](../README.zh-CN.md)
