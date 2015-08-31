---
layout: post
title: 几个css效果备忘
---
### 哀悼

	html {
		filter: grayscale(100%);//IE浏览器
		-webkit-filter: grayscale(100%);//谷歌浏览器
		   -moz-filter: grayscale(100%);//火狐
		    -ms-filter: grayscale(100%);
		     -o-filter: grayscale(100%);
		filter:progid:DXImageTransform.Microsoft.BasicImage(grayscale=1);
	}

### 禁止复制
	<div unselectable="on" onselectstart="return false;">
		sdfsdfswerwer324234234234
	</div>
