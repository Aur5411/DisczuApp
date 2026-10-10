# DisczuApp

适用于 **Discuz! X3.5** 论坛的 Android 客户端（WebView 壳）。

## 功能

- 桌面版浏览、阅读模式（字体 / 行距 / 主题 / 阅读进度）
- 附件下载：**自动重命名** —— 取帖子里的真实文件名，并去掉 `[sxsy.org]` / `soushu2025.com` / `@` 等站点标记
- 大文件（10MB 以上）TXT 下载：流式落盘，不爆内存
- 付费附件自动购买（可设单次价格上限）
- 广告与弹窗过滤、自动签到
- 多个常用网址一键切换，**各站登录状态互不影响**
- 自定义脚本：粘贴或导入本地 `.js`
- 下载目录默认 `Download/Discuz`（不存在自动创建）
- 首次启动需手动填写论坛网址，**无内置默认地址**
- 诊断日志（设置页连点「重置」5 次开启），便于排查下载问题

## 安装

从 Releases 下载 `Discuz-1.0.7-debug.apk` 安装即可。

- 包名：`com.discuz`
- 最低系统：Android 5.0（API 21）

> 换过包名，与旧版 `com.sxsy45.app` 无法共存，需先卸载旧版。

## 技术栈

Kotlin ｜ minSdk 21（Android 5.0）｜ targetSdk 34 ｜ JDK 21 + Gradle 8.14 + AGP 8.x ｜ AndroidX + 系统 WebView

## 编译

```bash
export JAVA_HOME=<JDK 21>
export ANDROID_HOME=<Android SDK>
gradle :app:assembleDebug
```

需要 Android SDK（compileSdk 34、build-tools 34）。

## 说明

仅供个人学习与自用；站点结构差异较大，个别功能可能需要按目标论坛调整。

## License

[MIT](./LICENSE)