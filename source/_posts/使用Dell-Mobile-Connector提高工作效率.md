---
title: 使用Dell Mobile Connector提高工作效率
date: 2019-03-19 14:47:38
tags: [Dell Mobile Connector, 日常工作]
categories:
---

# 使用Dell Mobile Connector提高工作效率

最近看《网络迷踪》，里面的人物可以在Mac电脑上打电话、发信息，真的让我很惊奇，google了一下，发现如果要实现那种情况，需要苹果全家桶。但以Windows作为工作环境的我，使用苹果全家桶几乎是不可能的。于是又google了一下，我发现Dell给出了解决方案，这就是Dell Mobile Connect。
## 什么是Dell Mobile Connect
Dell Mobile Connect可以无线连通 iOS、Android 和 Windows 三大平台，它不仅仅只是给你推送个来电或信息的通知，而是实实在在地让电脑手机连通协同工作，从而实现直接在 Windows 10 电脑上拨打/接听电话、收发短消息、查看联系人 (通讯录)，以及显示手机的推送通知。https://www.iplaysoft.com/dell-mobile-connect.html 有介绍。
Dell Mobile Connect可以说解决了一个我的痛点，
## 第一步，下载Dell Mobile Connector驱动
我的电脑是Dell XPS 9560，可以从DELL官网下载驱动，地址是 https://www.dell.com/support/home/cn/zh/cnbsd1/product-support/product/xps-15-9560-laptop/drivers 或者 https://www.dell.com/support/home/cn/zh/cnbsd1/drivers/driversdetails?driverId=6P0DG&osCode=WT64A&productCode=xps-15-9560-laptop, 安装驱动。
## 第二步，下载Dell Mobile Connect UWP程序
这个是UWP程序，但Microsoft Store中国区是没法下载的，我上传到百度网盘了，大家可以共享下.
链接: https://pan.baidu.com/s/1F9BWo4ck0PpVrPtMokQ-sQ 提取码: p2n2  
使用PowerShell打开如下命令进行安装
``` 
Add-AppxPackage -Path .\ScreenovateTechnologies.DellMobileConnect_1.2.6056.0_neutral_~_0vhbc3ng4wbp0.AppxBundle -DependencyPath .\Microsoft.VCLibs.140.00.UWPDesktop_14.0.25426.0_x64__8wekyb3d8bbwe.Appx 
```
安装后可以在开始菜单中打开Dell Mobile Connect快捷方式。
## 第三步，连接手机
我使用的是华为安卓手机，直接在华为应用市场内下载Dell Mobile Connect，打开蓝牙，安装成功后会出现连接码。在Windows10上打开Dell Mobile Connect，输入连接码，与手机连接成功后，即可在电脑上操作手机了，不用离开电脑，提高工作效率，爽歪歪

## 引用
> https://www.iplaysoft.com/dell-mobile-connect.html  
> https://www.reddit.com/r/Dell/comments/8zvn3u/howto_install_dell_mobile_connect_even_if_your/