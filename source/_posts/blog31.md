---
title: 修改软件图标和名称，改造你的手机桌面
author: JACK小桔子
categories: 安卓
date: 2020-09-04 21:16:30
top: false
tags: 
 - 软件
keywords: 软件
summary: 不想被人打开一个软件？试试修改它的图标和名称，别人绝对想不到这个软件的真面目！
img: /images/blog-cover/blog31.png
---
不想被人打开一个软件？试试修改它的图标和名称，别人绝对想不到这个软件的真面目！

### 第三方桌面
* 如果你是MIUI的手机，可以直接长按软件修改

1. 下载一个第三方桌面并安装打开(这里用的是[微软桌面](https://www.coolapk.com/apk/com.microsoft.launcher))，导入图标
![img1](/images/blog/blog31/img1.png "© JACK小桔子")
2. 长按即可修改图标和名称
![img2](/images/blog/blog31/img2.gif "© JACK小桔子")

### APK修改(非专业人员请离开)
1. 下载可以提取安装包的软件并安装打开(这里是[MT管理器](https://www.coolapk.com/apk/bin.mt.plus))
2. 点击左上角汉堡菜单，选择安装包提取，提取一个安装包，定位它的位置
3. 打开 - 查看安装包
![img3](/images/blog/blog31/img3.png "© JACK小桔子")
4. 打开里面的**AndroidManifest.xml**文件，选择反编译
![img4](/images/blog/blog31/img4.png "© JACK小桔子")
5. 找到`android:label=`，后面双引号里的内容就是名称，直接输入即可，点击保存
![img5](/images/blog/blog31/img5.gif "© JACK小桔子")
6. 这里一定要勾选**自动签名**，点击确定
![img6](/images/blog/blog31/img6.png "© JACK小桔子")
7. 打开下面四个文件夹：<br>
apk - res - mipmap-hdpi-v4<br>
apk - res - mipmap-xhdpi-v4<br>
apk - res - mipmap-xxhdpi-v4<br>
apk - res - mipmap-xxxhdpi-v4<br>
里面的**ic_launcher.png**都是图标，分别是4种大小，直接替换即可
![img7](/images/blog/blog31/img7.png "© JACK小桔子")
8. 最后重新安装即可
![img8](/images/blog/blog31/img8.png "© JACK小桔子")