---
title: 在电脑端多开微信
author: JACK小桔子
categories: Windows
date: 2020-07-12 20:02:31
top: false
tags: 
 - 软件
keywords: 微信
summary: 如果我们不止一个微信账号，但是又想在电脑上同时登陆，就只能使用多开的方法
img: /images/blog-cover/blog8.png
---
如果我们不止一个微信账号，但是又想在电脑上同时登陆，就只能使用多开的方法

### 微软应用商城
1. 如果你是用的是Windows10 系统，在下载官方微信后，还可以在微软应用商城搜索微信下载另一个版本的微信
![img1](/images/blog/blog8/img1.png "© JACK小桔子")
2. 这样你就有了2个微信
![img2](/images/blog/blog8/img2.png "© JACK小桔子")

### 批处理多开
1. 找到你微信的快捷方式，点击右键 → 属性
![img3](/images/blog/blog8/img3.png "© JACK小桔子")
2. 复制目标里的地址，**注意要把双引号也复制上**
![img4](/images/blog/blog8/img4.png "© JACK小桔子")
3. 新建一个记事本，随便起个名字，打开，里面输入以下内容
```bat
start "" [复制的内容]
start "" [复制的内容]
```
比如
```bat
start "" "C:\Program Files (x86)\Tencent\WeChat\WeChat.exe"
start "" "C:\Program Files (x86)\Tencent\WeChat\WeChat.exe"
```
![img5](/images/blog/blog8/img5.png "© JACK小桔子")
**要多开几个微信，就复制粘贴几行，这里就是多开2个微信**
4. 保存文件，将后缀名的txt改为bat(需要同意一下)
![img6](/images/blog/blog8/img6.png "© JACK小桔子")
![img7](/images/blog/blog8/img7.png "© JACK小桔子")
5. 双击运行即可
![img8](/images/blog/blog8/img8.png "© JACK小桔子")
* 如果懒得操作的话，可以在文章底部下载这个程序使用，**该程序已打包成exe文件**

![img9](/images/blog/blog8/img9.png "© JACK小桔子")

### 下载地址
* <font color = #bcbcbc>软件大小：</font><font color = #000000>143 KB</font>
* <font color = #bcbcbc>文件格式：</font><font color = #000000>exe</font>
* <font color = #bcbcbc>应用平台：</font><font color = #000000>Windows</font>

<font color = #ff0000>直链下载：</font>[点我传送](/resources/blog8/微信多开（2个）.exe)

<font color = #26a59a>蓝奏云盘：</font>[点我传送](https://xjz3103.lanzous.com/i2HRgejizmd)

<font color = #26a59a>百度云盘：</font>[点我传送](https://pan.baidu.com/s/11D7I_y5EqLACalrei-EApA)  `提取码: p4am`