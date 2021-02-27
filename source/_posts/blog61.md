---
title: Annie 视频下载工具使用方法
author: JACK小桔子

categories: 
 - Windows
date: 2021-02-27 20:41:33
top: false
tags: 
 - 软件
 - 技巧
 - Github项目
 - 程序
keywords: 视频下载
summary: Annie是一款使用Go构建的视频下载软件，无需安装，只需简单配置即可通过命令行快速解析下载国内外多平台视频，默认可支持最高分辨率。此工具支持MacOS、Windows以及Linux平台
img: /images/blog-cover/blog61.png
---
Annie是一款使用Go构建的视频下载软件，无需安装，只需简单配置即可通过命令行快速解析下载国内外多平台视频，默认可支持最高分辨率。此工具支持MacOS、Windows以及Linux平台，以下内容以Windows系统为例

### 安装方法
1. 打开该 [项目](https://github.com/iawia002/annie/releases) ,根据不同版本下载Annie
![img2](/images/blog/blog61/img2.png "© JACK小桔子")
2. Annie 基于 FFmpeg 下载合并，请到 [FFmpeg官网](https://www.ffmpeg.org/download.html) 选择系统下载
![img1](/images/blog/blog61/img1.png "© JACK小桔子")

> **注意**：FFmpeg不影响下载，仅影响最终文件合并

3. 将 Annie 放入 FFmpeg 的**bin**文件夹下，这个文件夹可以放在任意**固定**位置
![img3](/images/blog/blog61/img3.png "© JACK小桔子")

### 设置环境变量
1. 右击此电脑 - 属性 - 高级系统设置 - 环境变量
2. 在 系统变量 找到 Path文件 并点击编辑，点击新建
3. 将 Annie 的文件夹路径复制过来粘贴，一路确定即可
![img4](/images/blog/blog61/img4.gif "© JACK小桔子")
4. 检查环境：按下win + r，输入 cmd 确定，输入 Annie 回车，如果出现以下界面，说明安装成功
![img5](/images/blog/blog61/img5.gif "© JACK小桔子")

### 视频下载
打开 cmd 窗口，输入`Annie` + 空格 + 链接，回车即可下载，默认为最高分辨率
![img6](/images/blog/blog61/img6.gif "© JACK小桔子")
```cmd
Annie https://www.bilibili.com/video/BV1er4y1F7WC
```

Annie 支持B站短连接，可直接输入 AV号/BV号 下载
```cmd
Annie av755296319
Annie BV1er4y1F7WC
```

### 更改保存路径
1. 如果想要改变保存路径，可以输入cd + 空格 + 路径，回车即可
```cmd
cd D:
cd D:\annie
```
2. 或者打开你想保存的文件夹，在地址栏输入 cmd 回车，再输入视频下载命令即可
![img7](/images/blog/blog61/img7.gif "© JACK小桔子")
3. 你也可以在输入Annie后在输入 -o[小写] + 空格 + 路径 + 空格 + 链接，回车即可
```cmd
Annie -o desktop https://www.bilibili.com/video/BV1Rv4y1f7Xg
```

### 特殊功能
1. 在输入Annie后，输入-O[大写] + 空格 + 文件名 + 空格 + 链接，回车后就能修改视频名称
```cmd
Annie -O 测试 https://www.bilibili.com/video/BV1Rv4y1f7Xg
```
2. Annie的默认下载线程数为10，我们可以在输入Annie后，输入-n + 空格 + 线程数 + 空格 + 链接，回车就能改变下载线程
```cmd
Annie -n 32 https://www.bilibili.com/video/BV1Rv4y1f7Xg
```
3. 在输入Annie后，输入-i + 空格 + 链接，回车后就能查看视频的所有清晰度
```cmd
Annie -i https://www.bilibili.com/video/BV1Rv4y1f7Xg
```
4. 在输入Annie后，输入-p + 空格 + 链接，回车后就能下载整个视频列表
```cmd
Annie -p https://www.bilibili.com/video/BV1wE411176Q
```
5. 在输入Annie后，输入链接 + 空格 + 链接 + … ，可以同时下载多个视频
```cmd
Annie https://www.bilibili.com/video/BV1Rv4y1f7Xg https://www.bilibili.com/video/BV1Bi4y147hv
```

### 支持网站
| 网站         | 网址                           | 视频 | 图片 | 列表 | VIP |
|:------------:|:------------------------------:|:----:|:----:|:----:|:-----:|
| 抖音         | https://www.douyin.com     | ✓  |    |    |     |
| 优酷         | https://www.youku.com      | ✓  |    |    | ✓   |
| 秒拍         | https://www.miaopai.com    | ✓  |    |    |     |
| 微博         | https://weibo.com           | ✓  |    |    |     |
| 糖豆         | http://www.tangdou.com     | ✓  |    | ✓  |     |
| 爱奇艺        | https://www.iqiyi.com      | ✓  |    |    |     |
| 芒果TV       | https://www.mgtv.com       | ✓  |    |    |     |
| 半次元        | https://bcy.net             |    | ✓  |    |     |
| 音悦台        | https://yinyuetai.com       | ✓  |    |    |     |
| 斗鱼视频       | https://v.douyu.com        | ✓  |    |    |     |
| 哔哩哔哩       | https://www.bilibili.com   | ✓  |    | ✓  | ✓   |
| 腾讯视频       | https://v.qq.com           | ✓  |    |    |     |
| 极客时间       | https://time.geekbang.org  | ✓  |    |    |     |
| 好看视频       | https://haokan.baidu.com   | ✓  |    |    |     |
| 网易云音乐      | https://music.163.com      | ✓  |    |    |     |
| Twitter    | https://twitter.com         | ✓  |    |    |     |
| YouTube    | https://www.youtube.com    | ✓  |    | ✓  |     |
| pixivision | https://www.pixivision.net |    | ✓  |    |     |
| Facebook   | https://facebook.com        | ✓  |    |    |     |
| Instagram  | https://www.instagram.com  | ✓  | ✓  |    |     |

### 更多内容
* 单个视频下载
* 图片下载
* 多任务下载
* 短链接下载
* 查看资源信息
* 下载整个列表
* 多线程下载
* 指定下载路径
* 自定义代理
* 更多信息请查看 [Github项目](https://github.com/iawia002/annie)