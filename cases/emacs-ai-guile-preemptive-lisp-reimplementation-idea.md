# 重做Emacs运行时：AI辅助替换Elisp与抢占式LISP线程的引用idea

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-12
阶段：待验证

2026年11月12日11:36:12（北京时间），anya（@anya_tokugawa）引用文章讨论AI时代的Emacs重实现，具体方向为用Guile Scheme替换Emacs Lisp（Elisp），或实现抢占式LISP线程。Emacs是可用Lisp扩展的编辑器；目标是改造其运行时／并发限制，而非单纯换界面。

被引作者认为足够有兴趣的开发者凭100美元计划和长周末能做出不错的初稿。这是可行性意见，不是工时、预算或成功测量；计划的供应商和模型未给出，也不把没有人想做的评论当项目史事实。两个运行时方向属于同一Emacs重实现设想，未分别报告独立工程。

同段另引用The Emacsification of Software中AI定制Markdown查看器的故事，但没有给该查看器的逆向对象或功能重建证据，因此不另算案例。补取确认发帖人与引用文本；文章正文、原作者、源码、兼容性和线程测试均未核，不能说已经替换Elisp、保留全部插件或达成线程安全。本合集未运行编辑器或生成实现。

封存候选0赞、20浏览、0转发；100美元与长周末是引用中的估计，不是实际投入。

## 来源

- [anya引用的Emacs运行时重实现idea，2026-11-12 11:36:12北京时间](https://x.com/i/status/2120722301171966025)

[English](en/emacs-ai-guile-preemptive-lisp-reimplementation-idea.md) | [返回目录](../README.zh-CN.md)
