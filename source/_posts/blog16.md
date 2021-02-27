---
title: win10重装系统
author: JACK小桔子
categories: Windows
date: 2020-08-19 9:51:45
top: false
tags: 
 - 系统
keywords: 系统
summary: 最近电脑总是出现奇怪的问题，最后决定重装系统，顺便记录重装过程。
img: /images/blog-cover/blog16.jpg
---
最近电脑总是出现奇怪的问题：C 盘空间突然减少直至 0 字节可用；开始菜单出现问题 …… 😓最后决定重装系统，顺便记录重装过程。
### 下载镜像
#### msdn网站
1. 在 [msdn](https://msdn.itellyou.cn/) 这个网站下载，展开`操作系统`
![img1](/images/blog/blog16/img1.png "© JACK小桔子")
2. 点击一个版本后面的`详细信息`，复制以**ed2k://**开头的链接
![img2](/images/blog/blog16/img2.png "© JACK小桔子")
3. 打开迅雷粘贴链接即可

#### 官网镜像下载
* 打开[微软官网](https://www.microsoft.com/zh-cn/software-download/windows10)，可以下载媒介工具，使用媒介工具下载系统镜像，但是相对麻烦，而且有速度限制。<font color=#26a59a>使用下面的方法，就可以在官网直接下载系统镜像</font>
![img3](/images/blog/blog16/img3.png "© JACK小桔子")
1. 按下F12，点击**切换设备工具栏**，切换设备到**iPad Pro**
![img4](/images/blog/blog16/img4.png "© JACK小桔子")
2. 刷新页面，**等待网页加载完成后**关闭审查元素，可以看到页面多出了版本和语言选择
![img5](/images/blog/blog16/img5.png "© JACK小桔子")
3. 选择选择版本、语言和64位或32位，下载即可
![img6](/images/blog/blog16/img6.png "© JACK小桔子")

### 进入PE系统
#### 下载PE系统
1. 这里使用[微pe工具箱](http://www.wepe.com.cn/)，下载后运行，点击下方的U盘按钮
![img7](/images/blog/blog16/img7.png "© JACK小桔子")
2. 根据情况选择参数，点击`立即安装到U盘`
![img8](/images/blog/blog16/img8.png "© JACK小桔子")
3. 将之前下载好的win10镜像拷贝进U盘**(只要镜像不在系统盘就行)**
4. 关闭电脑，开机的时候进入BIOS，一般是按下`Del`按键(不同主板的快捷键不同，可以自行百度)
![img9]( "© JACK小桔子")
5. 在Boot中将U盘移至第一位，保存并重启(此步骤不同主板的方法不同，可以自行百度)
![img10]( "© JACK小桔子")
6. 重启后就进入PE系统了
    1. 建议先使用**DiskGenius**先格式化系统盘
    ![img11](/images/blog/blog16/img11.jpg "© JACK小桔子")
    2. 打开U盘，右键系统镜像，点击装载
    ![img12](/images/blog/blog16/img12.jpg "© JACK小桔子")
    3. 双击运行**Setup.exe**，根据需要配置参数，可参考下图
    ![img13](/images/blog/blog16/img13.jpg "© JACK小桔子")
    4. 安装完成后重启电脑

### 安装系统
* 这个过程会重启数次
* 根据需要选择参数即可

### 激活系统
1. 下载激活工具[CMWTAT](https://github.com/TGSAN/CMWTAT_Digital_Edition/releases)，觉得下载速度慢的可以用这个链接：[点我传送](https://xjz3103.lanzoux.com/iRzxZfsqrja) (我的蓝奏云)
2. 运行程序，点击激活即可
![img14](/images/blog/blog16/img14.png "© JACK小桔子")