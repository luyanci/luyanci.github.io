---
title: Magisk安装教程
date: 2023-06-29 17:52:01
tags: 软件
cover: /image/magisk/magisk.webp
---
# [视频教程](https://www.bilibili.com/video/BV13B4y1x7rh)
<iframe src="//player.bilibili.com/player.html?aid=600285833&bvid=BV13B4y1x7rh&cid=756404306&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

# 文字教程
**前提：手机已经解锁BL**
## 获取系统boot镜像
以MIUI系统为例 打开设置-我的设备-全部参数来查询自己的系统版本号
![](/image/magisk/1.jpg) 
查询完后到[XiaomiROM](https://xiaomirom.com)找该版本的完整卡刷包并下载
双击打开卡刷包，如果有boot.img就直接解压，如果没有但有payload.bin，则需要找工具解包(这里不想多讲)
**近期出的手机可能会因为修补boot.img导致无法进入系统（甚至报系统损坏），搞机需谨慎哦**
## 修补并刷入boot
安装[面具](https://github.com/topjohnwu/magisk/releases)，点击上面的安装，选择提取的boot镜像,然后点开始
等待一会，如果显示done,就可以把修补后的文件传回到电脑里
打开命令提示符（cmd/powershell）输入以下命令
``` 
For cmd
fastboot flash boot <boot image>
For PowerShell
./fastboot flash boot <boot image>
```
刷入成功后重启，打开面具，magisk栏显示版本号，代表刷入成功
>文章相关资源
[小米解锁](https://www.miui.com/unlock/index.html) 
[​adb工​具](https://developer.android.google.cn/studio/releases/platform-tools) 
[面具](https://github.com/topjohnwu/Magisk/releases)
 [xiaomiroms](https://xiaomirom.com/) 
[面具中文网](https://magiskcn.com)