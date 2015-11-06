---
layout: post
title: OS X 中 更新 Eclipse Luna 后无法启动
---

今天我更新 Eclipse 后发现无法启动，提示需要jvm1.6才能运行，点击确定后自动安装了jvm1.6。

再次双击 Eclipse 依然报错，不过这次是「Version 1.6.0_65 of the JVM is not suitable for this product.」，这就是个坑。你说要1.6我照你做安装了1.6，还是你帮我自动装的，装完你告诉我不行……

报错信息还有下半部分「Version: 1.7 or greater is required.」好吧，那我去下载1.7吧。

下载完 jre1.7，安装后在系统偏好设置里可以看到 jre 的版本号已经是 1.7了，双击运行依然报错……

Google 了半天，中英文都试了，基本就没有成功案例。所以我只能碰运气了，于是下载了 jdk-7u60-macosx-x64，双击一试居然成了。