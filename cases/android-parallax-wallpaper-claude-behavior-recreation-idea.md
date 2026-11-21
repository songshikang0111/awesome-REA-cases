# 三层视差动态壁纸：Claude提示重建Android倾斜效果，而非APK破解

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-22
阶段：待验证

2026年11月22日03:37（北京时间），一则英文帖子以Android逆向作开头，随后给出Claude提示：用Kotlin、WallpaperService和Canvas引擎做3D视差壁纸，不用第三方库。三个PNG层读TYPE_ROTATION_VECTOR，低通平滑，背景、光晕、前景按5%、12%、25%移动，前景反向；加随倾斜变化的阴影、70%至100%的四秒呼吸透明度、0.5至2倍深度滑块。

提示还要求可见时60fps、不可见时注销传感器，并输出manifest、wallpaper.xml、代码与构建指导。这些是请求规格，不是生成结果或实测帧率、省电数据。没有具名原应用、APK、私有API或逆向轨迹，不能称已破解动态壁纸；AI抠图只是素材建议。作为复建可观察壁纸效果的具体idea收录，未执行提示、安装应用或采集传感器数据，REA未提，状态unverified。

## 来源

- [Claude重建Android三层视差壁纸的提示，2026-11-22 03:37北京时间](https://x.com/i/status/2124225587623473600)

[English](en/android-parallax-wallpaper-claude-behavior-recreation-idea.md) | [返回目录](../README.zh-CN.md)
