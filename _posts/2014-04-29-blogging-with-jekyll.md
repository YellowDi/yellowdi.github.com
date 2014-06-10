---
layout: post
title: 使用 Github Pages 建博客
---
利用 [Github Pages](https://pages.github.com/) 和 [Jekyll](http://jekyllrb.com/) 搭建一个静态博客的教程网上到处是，以下只是我自己的一种方法，适用于安装过 [Github for Mac](https://mac.github.com/) 客户端的人，只需要拖拖拽拽就可以搭建一个博客，完全不需要使用终端命令。不能保障其他平台是否适用此方法，我也没法亲自尝试。

### 第一步

首先你需要一个 [Github](http://github.com) 帐号，假设你叫「xxxx」，那么创建一个名为 「xxxx.github.com」的 Repository。

随后进入项目设置 「github.com/xxxx/xxxx.github.com/settings」找到「GitHub Pages」选项一路下一步创建一个预设模板的页面。

如果顺利的话十分钟内你就能访问「xxxx.github.com」看到页面内容了。

然后我们进行下一步，「**Clone in Desktop**」

随后查看你的 Finder 中是否有了名为「xxxx.github.com」的文件夹，如果有需要你清空文件夹并顺利进入下一步。

### 第二步

接下来的教程除了部署 Jekyll 还安装了我现在正在用的模板：[Scribble](https://github.com/muan/scribble)

![screenshot](http://scribble.muan.co/images/screenshot.png)

过程同样非常简单，进入「Scribble」的项目页面点击「**Download ZIP**」下载，解压至「xxxx.github.com」文件夹并修改「_config.yml」和「about.md」

### 第三步

打开「Github for Mac」进入「xxxx.github.com」你会看到 「Changes」有了很多修改，接下来你只需要撰写一下发布说明按下「Commit & Sync」稍等片刻，项目就上传至 Github 了。

至此，利用 [Github Pages](https://pages.github.com/) 和 [Jekyll](http://jekyllrb.com/) 搭建一个静态博客的全部流程到这里也就结束了。

