---
layout: post
title: 微信视频自动播放不全屏
---
在 video 标签中加入 webkit-playsinline="true" 已放置 iOS 自动进入全屏播放。引入微信 sdk 并添加 document.getElementById('myVideo').play(); 自动播放，特殊情况也可以用
  document.addEventListener("WeixinJSBridgeReady", function() {
    document.getElementById('myVideo').play();
  }, false);
  实现
