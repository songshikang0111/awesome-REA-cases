# AIUP的PetClinic示例：从旧代码恢复用例规格，再渐进维护

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-05
阶段：相关项目

2026年11月5日02:35:56（北京时间），Simon Martinelli（@simas_ch）介绍AI Unified Process（AIUP）新增brownfield部分：面对先有多年代码、原作者可能离开的系统，先从现有代码逆向用例图、用例规格与实体模型，再由Requirements Engineer和Software Engineer共同纠错、记开放问题。审查后接受当前发现为基线，只让新问题阻断构建，并记录现有技术栈，不要求先迁框架。

其维护路线是在原栈协调规格与代码，不整库重新生成；现代化路线则把旧系统作为需求来源，逐用例、逐模块迁移。具体展示是Spring PetClinic，作者称start分支为逆向后状态，main为所有用例已实现并测试，承认例子很小，更大例子仍是计划。

未取得可确认仓库、分支差异、规格、测试日志、模型或Agent执行记录。没有既有测试也能起步是流程主张；从恢复规格生成的测试不能独立证明规格等于原行为，失败也不必然是产品缺陷。按AI相关源码到规格恢复项目收录，不称二进制反编译或已证明大型系统迁移有效；未运行代码，REA未提。

封存4赞、245浏览、3转发；start／main状态均为作者说法，未核验分支。

## 来源

- [Simon Martinelli的AIUP旧系统流程与PetClinic展示，2026-11-05](https://x.com/i/status/2118049623906648130)

[English](en/aiup-spring-petclinic-brownfield-spec-recovery.md) | [返回目录](../README.zh-CN.md)
