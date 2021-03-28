---
title: Inno Setup(安装包制作软件)增强版
author: JACK小桔子
categories: 
 - Windows
date: 2020-12-27 18:53:20
top: false
tags: 
 - 软件
 - VIP
keywords: 安装包
summary: Inno Setup是一款Windows免费的安装制作软件，Inno Setup功能强大，制作快速，对于一般的Windows安装制作都能够快速地完成，并且Inno Setup软件小巧、操作简便、界面精美，功能齐全，受到了很多用户的喜爱，是一款很实用的安装制作软件
img: /images/blog-cover/blog69.png
---
Inno Setup是一款Windows免费的安装制作软件，Inno Setup功能强大，制作快速，对于一般的Windows安装制作都能够快速地完成，并且Inno Setup软件小巧、操作简便、界面精美，功能齐全，受到了很多用户的喜爱，是一款很实用的安装制作软件

**<center>@ 风铃夜思雨</center>**

### 打包教程
1. [下载](/2020/12/27/blog69/#下载地址) 安装并打开 Inno setup 编辑器软件，点击文件 - 新建
![img1](/images/blog/blog69/img1.png "© JACK小桔子")
2. 点击下一步
![img2](/images/blog/blog69/img2.png "© JACK小桔子")
3. 填写好基本信息，点击下一步
![img3](/images/blog/blog69/img3.png "© JACK小桔子")
4. 这里基本不用更改，点击下一步
![img4](/images/blog/blog69/img4.png "© JACK小桔子")
5. 在上方选择主执行文件；在下方添加软件的文件夹；点击下一步
    * 主执行文件：安装完成后默认打开的文件
    * 其他应用程序文件：整个软件的文件夹
![img5](/images/blog/blog69/img5.png "© JACK小桔子")
6. 在这里设置相应功能，点击下一步
![img6](/images/blog/blog69/img6.png "© JACK小桔子")
7. 在这里设置安装包的权限，点击下一步
    * 上方选择是否以管理员身份安装
    * 允许用户通过命令行覆盖安装方式：是否用命令行(cmd)安装
    * 在启动时要求用户选择安装模式：再打开安装包时询问是否以管理员身份安装
![img7](/images/blog/blog69/img7.png "© JACK小桔子")
8. 在这里可以安装输出的文件夹，软件名称以及软件图标，点击下一步
![img8](/images/blog/blog69/img8.png "© JACK小桔子")
9. 选择安装的语言(可多选)，点击下一步
10. 在这里选择编译后安装包的输出文件夹，输出文件名等，还可以加载自定义的安装程序图标，点击下一步
![img9](/images/blog/blog69/img9.png "© JACK小桔子")
11. 选择 是否使用define编译指令 ，点击下一步，然后点击完成
12. 然后选择是否编译这个脚本，如果选择是，将会让你保存脚本并编译
![img10](/images/blog/blog69/img10.png "© JACK小桔子")
13. 在这里你可以随时修改脚本
![img11](/images/blog/blog69/img11.png "© JACK小桔子")

本软件脚本：
```iss
; 脚本由 Inno Setup 脚本向导 生成！
; 有关创建 Inno Setup 脚本文件的详细资料请查阅帮助文档！

#define MyAppName "测试"
#define MyAppVersion "1.0"
#define MyAppPublisher "JACK小桔子"
#define MyAppURL "https://jackxjz.vercel.app/"
#define MyAppExeName "SoundBooster.exe"

[Setup]
; 注: AppId的值为单独标识该应用程序。
; 不要为其他安装程序使用相同的AppId值。
; (若要生成新的 GUID，可在菜单中点击 "工具|生成 GUID"。)
AppId={{7C69C16B-F600-4594-B7AD-A02F07705F34}
AppName={#MyAppName}
AppVersion={#MyAppVersion}
;AppVerName={#MyAppName} {#MyAppVersion}
AppPublisher={#MyAppPublisher}
AppPublisherURL={#MyAppURL}
AppSupportURL={#MyAppURL}
AppUpdatesURL={#MyAppURL}
DefaultDirName={autopf}\{#MyAppName}
DefaultGroupName={#MyAppName}
AllowNoIcons=yes
InfoBeforeFile=D:\3思杰文档\等级4-编辑器\0安装包制作\说明文件.txt
; 以下行取消注释，以在非管理安装模式下运行（仅为当前用户安装）。
;PrivilegesRequired=lowest
PrivilegesRequiredOverridesAllowed=dialog
OutputBaseFilename=SoundBooster - JACK小桔子
Compression=lzma
SolidCompression=yes
WizardStyle=modern

[Languages]
Name: "chinesesimp"; MessagesFile: "compiler:Default.isl"

[Tasks]
Name: "desktopicon"; Description: "{cm:CreateDesktopIcon}"; GroupDescription: "{cm:AdditionalIcons}"; Flags: unchecked

[Files]
Source: "D:\Program Files\SoundBooster\SoundBooster.exe"; DestDir: "{app}"; Flags: ignoreversion
Source: "D:\Program Files\SoundBooster\*"; DestDir: "{app}"; Flags: ignoreversion recursesubdirs createallsubdirs
; 注意: 不要在任何共享系统文件上使用“Flags: ignoreversion”

[Icons]
Name: "{group}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"
Name: "{group}\{cm:UninstallProgram,{#MyAppName}}"; Filename: "{uninstallexe}"
Name: "{autodesktop}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"; Tasks: desktopicon

[Run]
Filename: "{app}\{#MyAppExeName}"; Description: "{cm:LaunchProgram,{#StringChange(MyAppName, '&', '&&')}}"; Flags: nowait postinstall skipifsilent
```

### 修改说明
@风铃夜思雨
* 包含Ansi和Unicode版本。
* 加入加密组件ISCrypt.dll。
* 加入Inno Setup预处理器。(可选择安装)
* 加入一些辅助工具。(可选择安装)

### 下载地址
* <font color = #bcbcbc>软件大小：</font><font color = #000000>29.0 MB</font>
* <font color = #bcbcbc>文件格式：</font><font color = #000000>zip</font>
* <font color = #bcbcbc>应用平台：</font><font color = #000000>Windows</font>
* <font color = #bcbcbc>文件版本：</font><font color = #000000>6.0.5</font>

<font color = #26a59a>蓝奏云盘：</font>[点我传送](https://xjz3103.lanzoux.com/iRsNtjrynqj)

<font color = #26a59a>百度云盘：</font>[点我传送](https://pan.baidu.com/s/1FIiTOhDQ0BU7mtNujlSwXQ)  `提取码: nd6x`

<font color = #26a59a>坚果云盘：</font>[点我传送](https://www.jianguoyun.com/p/Dd7NctsQ8tX5CBi_ndUD)

<font color = #26a59a>天翼云盘：</font>[点我传送](https://cloud.189.cn/t/3IRJnifQJNfa)  `访问码: ise4`

<font color = #26a59a>奶牛快传：</font>[点我传送](https://cowtransfer.com/s/cc86c1c09df94a)  `收件码: 056807`