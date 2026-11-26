# Emerald NX：AI辅助Switch原生移植的介绍，首次真机启动仍待测

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-27
阶段：进行中

2026年11月27日01:12:01（北京时间），The Gaming Emporium（@TheEmporium83）介绍eonlynx发布的Emerald NX v0.5.0：基于pret/pokeemerald反编译及已有Emerald 3DS、Android引擎，把《宝可梦绿宝石》原生移到Switch，并称开发者确认大量使用AI辅助。这是介绍者的AI归因，没有取得开发者模型会话，不能把pret既有反编译归功于本次AI移植。

补读eonlynx/emerald-nx固定a64db5d03de9e430157753314bf21656d91b3904的README和2026年11月25日最终审计；该提交时间为11月26日15:03:49 UTC，早于本窗口，文档仅作补充证据。项目描述libnx与GLES3、低于4GiB地址的两级NRO加载器、720p掌机／1080p底座输出、单屏触控布局、可选体素场景和跨ARM32／AArch64存档布局检查。体素模式默认关闭，大量地图和室内仍平面，本地无线为stub。

重要限制比介绍中的发布措辞更严格：README明确最终包尚未在主机运行，首次硬件测试待做。审计报告完整AArch64构建和打包通过、存档布局及13项overlay例外已检查，不等于画面、音频、存档迁移或整游戏在真机验证。原帖还列跟随宝可梦、物特分离、无限TM等继承功能，并非本次AI独立发明。须有合法游戏来源；构建生成的pak即使不是ROM仍含游戏内容，不能据无ROM宣称自由分发。这里只读文档，未下载游戏数据、安装依赖、构建或运行，状态in-progress。

候选封存19赞、813浏览、3转发、0回复；v0.5.0为介绍帖版本，AI模型未指明。

## 来源

- [The Gaming Emporium的Emerald NX与AI辅助介绍，2026-11-27 01:12:01北京时间](https://x.com/i/status/2126001039723639201)
- [窗口前补充固定README：首次硬件启动待测，提交2026-11-26 15:03:49 UTC](https://github.com/eonlynx/emerald-nx/blob/a64db5d03de9e430157753314bf21656d91b3904/README.md)
- [同修订11月25日构建／静态审计文档，不是本合集重跑](https://github.com/eonlynx/emerald-nx/blob/a64db5d03de9e430157753314bf21656d91b3904/switch_port/FINAL_AUDIT_2026-11-25.md)

[English](en/emerald-nx-ai-assisted-switch-native-port.md) | [返回目录](../README.zh-CN.md)
