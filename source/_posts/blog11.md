---
title: 去网页广告
author: JACK小桔子
categories: 浏览器
date: 2020-07-16 09:15:00
top: false
tags: 
 - 美化
summary: 在我们浏览网页的时候，经常会看到各种各样的广告，有些可以去除，但是如果广告一多就很不方便了；有些无法去除，很影响上网体验。使用这个插件可以将广告全部去除！
img: /images/blog-cover/blog11.png
---
> 在我们浏览网页的时候，经常会看到各种各样的广告，有些可以去除，但是如果广告一多就很不方便了；有些无法去除，很影响上网体验。使用这个插件可以将广告全部去除！

其实去除广告的插件不少，个人认为uBlock是最好用的一个。

### 安装使用
1. 你需要能访问谷歌，如果还不能翻墙的可以看这篇文章：[点我传送](https://jackxjz.vercel.app/2020/06/19/blog2/)
去广告插件安装连接：[点我传送](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)
2. 打开此链接，点击右边的添加至Chrome，点击添加扩展程序，稍等片刻即可
![img1](/images/blog/blog11/img1.png "© JACK小桔子")

### 基本使用
1. 启动插件，默认全局拦截
![img2](/images/blog/blog11/img2.png "© JACK小桔子")
2. 我们也可以手动添加过滤的元素。比如把整个侧边删除，只需点击插件，点击吸管，选择它的区域，点击创建即可
![img3](/images/blog/blog11/img3.gif "© JACK小桔子")
* 恢复某个手动添加的过滤元素需要点击插件，打开设置，选择自定义静态规则，在这里可以删除
![img4](/images/blog/blog11/img4.gif "© JACK小桔子")

### 添加脚本
其实它也是个载体框架，就像tampermonkey和用户写的脚本的关系。它内置了很多自带的规则，可以根据个人喜好开启或关闭这些功能。
![img5](/images/blog/blog11/img5.png "© JACK小桔子")
1. 打开这个网址:[点我传送](https://filterlists.com/)，里面有很多大佬编写的规则
![img6](/images/blog/blog11/img6.png "© JACK小桔子")
2. 点击语言旁边的筛选，可以选择国家，查看该国比较不错的规则
![img7](/images/blog/blog11/img7.png "© JACK小桔子")
3. 点击规则旁的图标，选择添加，就可以添加到uBlock中，这时我们再回到控制面板，就可以看到刚刚添加的规则了
![img8](/images/blog/blog11/img8.png "© JACK小桔子")
4. 当然我们也可以手动加载，我搜集了一些规则链接，点击导入，粘贴网址即可
![img9](/images/blog/blog11/img9.png "© JACK小桔子")

### 去视频广告
uBlock还可以轻松去除120秒的视频片头广告，在安装完乘风视频广告过滤规则后，爱奇艺，优酷，腾讯视频的广告都可以拦截，直接开始观看
![img10](/images/blog/blog11/img10.gif "© JACK小桔子")