---
title: 如何删除磁盘列表中的快捷方式
author: JACK小桔子
categories: 
 - Windows
date: 2020-09-18 20:17:47
top: false
tags: 
 - 技巧
keywords: 实用技巧
summary: 我的电脑磁盘总是出现一些快捷方式，比如百度网盘/WPS网盘等，对于强迫症来说是绝对不能忍受的，用这个方法可以100%删除这些快捷方式
img: /images/blog-cover/blog40.png
---
我的电脑磁盘总是出现一些快捷方式，比如百度网盘/WPS网盘等，对于强迫症来说是绝对不能忍受的，用这个方法可以100%删除这些快捷方式

![img1](/images/blog/blog40/img1.png "© JACK小桔子")

### 软件设置关闭
这里以百度网盘为例，打开设置，这里就可以选择关闭了
![img2](/images/blog/blog40/img2.png "© JACK小桔子")

### 注册表移除
如果软件设置里没有此选项，可以在注册表中删除
1. 按下Win + R 打开运行，输入`regedit`回车打开注册表
![img3](/images/blog/blog40/img3.png "© JACK小桔子")
2. 找到`HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\MyComputer\NameSpace\`
3. 删除`NameSpace`下的所有内容即可
![img4](/images/blog/blog40/img4.png "© JACK小桔子")
4. 重新打开我的电脑，可以看到所有快捷方式都消失了
![img5](/images/blog/blog40/img5.png "© JACK小桔子")