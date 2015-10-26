---
layout: post
title: 微信视频自动播放不全屏
---
<video preload="auto" loop="" webkit-playsinline="true" muted="" poster="images/header.ef9f192a.jpg" class="hidden-xs" id="myVideo">
  <!-- <source data-src="images/polina.webm" type="video/webm" /> -->
  <source src="http://www.yunmodel.com/video/low-bg.11852c36.mp4" type="video/mp4"> </video>

<script src="http://res.wx.qq.com/open/js/jweixin-1.0.0.js"></script>
<script>
  //一般情况下，这样就可以自动播放了，但是一些奇葩iPhone机不可以
  document.getElementById('myVideo').play();
  //必须在微信Weixin JSAPI的WeixinJSBridgeReady才能生效
  document.addEventListener("WeixinJSBridgeReady", function() {
    document.getElementById('myVideo').play();
  }, false);
</script>
