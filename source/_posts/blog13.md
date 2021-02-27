---
title: 任意修改网页内容
author: JACK小桔子
categories: 浏览器
date: 2020-07-21 12:44:50
top: false
tags: 
 - 程序
summary: 你想不想拥有随意改网页上内容的“超能力”呢？一起来看看吧
img: https://cdn.jsdelivr.net/gh/xjz3103/cdn@1.4/img/cover/blog13.png
---
<iframe src="//player.bilibili.com/player.html?aid=456434418&bvid=BV1c5411a7tU&cid=215249908&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

> 你想不想拥有随意改网页上内容的“超能力”呢？一起来看看吧

1. 在一个网页按下**F12**，或者右键 - 检查，打开开发人员面板

![img1](https://s1.ax1x.com/2020/07/21/UoyBPP.png "© JACK小桔子")

2. 切换到控制台面板(Console面板)

![img2](https://s1.ax1x.com/2020/07/21/Uo61ds.png "© JACK小桔子")

3. 在这里输入以下指令并按回车，当出现`undefined`就成功了
```js
javascript:document.body.contentEditable='true'; document.designMode='on'; void 0
```

![img3](https://s1.ax1x.com/2020/07/21/UocSkn.png "© JACK小桔子")

看看效果：
![img4](https://s1.ax1x.com/2020/07/21/Uo2CsU.gif "© JACK小桔子")