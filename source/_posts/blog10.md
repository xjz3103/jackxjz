---
title: 图片背景二维码
author: JACK小桔子
categories: Windows
date: 2020-07-12 09:50:13
top: false
tags: 
 - 程序
 - Python
keywords: 二维码
summary: 我们的生活中充满了各式各样的二维码，但是你有见过以图片为背景的二维码吗？
img: /images/blog-cover/blog10.png
---
我们的生活中充满了各式各样的二维码，但是你有见过以图片为背景的二维码吗？
![img1](/images/blog/blog10/img1.png "© JACK小桔子")

### 安装python
1. 打开[python官网](https://www.python.org/)，**将鼠标放在**downloads上(**不要点击downloads**)，它会自动识别你的操作系统并给出下载按钮，点击即可
![img2](/images/blog/blog10/img2.png "© JACK小桔子")

* 从官网下载速度很慢，可以在这个[这个网址](https://npm.taobao.org/mirrors/python/)下载，这是国内的镜像源，选择最新版本的python，选择操作系统下载即可
![img3](/images/blog/blog10/img3.png "© JACK小桔子")
2. 安装前**一定**要勾选上“Add Python [版本号] to PATH选项”，点击“Install Now”，安装完成后点击“Close”即可
![img4](/images/blog/blog10/img4.png "© JACK小桔子")

### 安装myqr组件
1. 打开命令提示符：按下windows + r ，输入cmd点击确定；或者搜索命令提示符打开
![img5](/images/blog/blog10/img5.png "© JACK小桔子")
![img6](/images/blog/blog10/img6.png "© JACK小桔子")
2. 在cmd中输入：
```python
pip install myqr
```
在运行结果中看到“Successfully installed”说明安装成功

### 使用myqr
#### 文字二维码
1. 打开你需要制作二维码的背景图所在的文件夹，在地址栏输入cmd (用cmd打开此文件夹)
![img7](/images/blog/blog10/img7.png "© JACK小桔子")
2. 在这个窗口输入
```python
myqr -c -v[边长] -p [图片地址] [二维码文字/网址]
```
比如
```python
myqr -c -v20 -p 图片.jpg 壁纸
```
* 其中 -c 表示使用彩色制作二维码
3. 按下回车，当出现“Succeed！”说明制作成功，回到该图片文件夹即可看到

#### 链接二维码
我们还可以把微信支付/加好友的二维码加上图片背景
1. 从微信下载微信支付/加好友的二维码
![img8](/images/blog/blog10/img8.png "© JACK小桔子")
2. 打开[草料二维码](https://cli.im/deqr/)，解析二维码，将结果复制下来
![img9](/images/blog/blog10/img9.png "© JACK小桔子")
3. 打开你需要制作二维码的背景图所在的文件夹，在地址栏输入cmd ，在弹出的窗口中窗口输入
```python
myqr -c -v[边长] -p [图片地址] [复制的网址]
```
比如
```python
myqr -c -v20 -p 图片.jpg https://u.wechat.com/MAItx2f53bl0X9quBhnFQWA
```
4. 最终效果，**有兴趣的可以扫一扫~**
![img10](/images/blog/blog10/img10.png "© JACK小桔子")