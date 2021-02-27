---
title: win7激活
author: JACK小桔子
categories: Windows
date: 2020-8-22 09:23:46
top: false
tags: 
 - 系统
keywords: 系统
summary: 都2020年了，你还不会激活win7？！
img: /images/blog-cover/blog17.jpg
---
都2020年了，你还不会激活win7？！相信很多人都是用激活工具激活的吧？这里介绍如何不用任何工具，不用一分钱激活win7

### win7旗舰版
1. 右键计算机，点击属性，点击产品ID右侧的`更改产品密钥`
![img1](/images/blog/blog17/img1.png "© JACK小桔子")
2. 在下方的3个密钥中复制一个，输入到产品密钥，点击下一步
```
K94XV-CGT4P-P72FP-D79DV-8XHG9
BRKJB-DV2BP-MBBPW-7FVQ4-G3QYR
YM8MJ-JKTGM-8GFQ6-X499R-FT7V7
```
![img2](/images/blog/blog17/img2.png "© JACK小桔子")
3. 如果验证产品密钥失败，点击`使用自动的电话系统来激活`
![img3](/images/blog/blog17/img3.png "© JACK小桔子")
4. 位置选择中国
5. 打开这个网址：[点我传送](https://webact.185.hk/)，将安装ID输入到网站的对应位置，点击提交
![img4](/images/blog/blog17/img4.png "© JACK小桔子")
6. 将网站上的确认ID输入到Windows激活的对应位置，点击下一步
![img5](/images/blog/blog17/img5.png "© JACK小桔子")
7. 这样就激活了
![img6](/images/blog/blog17/img6.png "© JACK小桔子")

### win7专业版
1. 打开开始菜单 - 所有程序 - 附件，右键命令提示符，点击`以管理员身份运行`
2. 依次输入下方4条指令即可
```bat
slmgr.vbs -upk
slmgr.vbs -ipk FJ82H-XT6CR-J8D7P-XQJJ2-GPDD4 
slmgr.vbs -skms kms.cangshui.net  
slmgr.vbs -ato
```