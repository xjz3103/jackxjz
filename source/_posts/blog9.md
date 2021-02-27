---
title: 强制结束进程
author: JACK小桔子
categories: Windows
date: 2020-07-12 08:31:29
top: false
tags: 
 - PowerShell
keywords: 结束进程
summary: 在使用Windows系统的过程中，都会碰到过应用程序卡死的情况。通常情况下，我们会使用任务管理器结束进程，不过，有时候连任务管理器也没有办法，这时我们可以尝试使用PowerShell
img: /images/blog-cover/blog9.png
---
在使用Windows系统的过程中，都会碰到过应用程序卡死的情况。通常情况下，我们会使用任务管理器结束进程，不过，有时候连任务管理器也没有办法，这时我们可以尝试使用PowerShell

1. 右键任务栏，点击任务管理器；或者使用快捷键Ctrl+Shift+Esc
![img1](/images/blog/blog9/img1.png.png "© JACK小桔子")
2. 点击详细信息，找到卡死的应用，就可以看到它的PID值(这里是微信)
![img2](/images/blog/blog9/img2.png.png "© JACK小桔子")
3. 右键开始按钮，点击Windows PowerShell(管理员)
![img3](/images/blog/blog9/img3.png.png "© JACK小桔子")
4. 在弹出的窗口中输入
```PowerShell
tskill [PID值]
```
比如
```PowerShell
tskill 9120
```
![img4](/images/blog/blog9/img4.png.png "© JACK小桔子")
5. 按下回车即可
![img5](/images/blog/blog9/img5.png.png "© JACK小桔子")
* 这个方法适用于所有Windows系统
