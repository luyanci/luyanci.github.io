---
title: LSPosed安装
date: 2023-07-01 16:17:20
tags: 软件
cover: /image/lsposed/top.webp
---
# 简单介绍
LSPosed是目前主流的XPosed框架，支持**安卓8.1-13**

## **桌面找不到图标？**
**自1.8.6版本LSPosed起，默认入口就更改到了通知栏位置(记得往下拉哦)**
如果实在找不到的话就拨号盘暗码(*#*#5776733#*#*)来进入管理器
进入管理器后就可以点设置手动把桌面图标弄出来啦~

# [视频教程](https://www.bilibili.com/video/BV13B4y1x7rh)
<iframe src="//player.bilibili.com/player.html?aid=685579245&bvid=BV1dU4y1S7AY&cid=763587977&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

# 文字教程（以最新稳定为例）
## 下载
打开[LSPosed的Github页面](https://github.com/LSPosed/LSPosed/)，直接找到releases，下载**magisk模块**包
**这里下载的是模块包，不是管理器！**
打不开github的可以试试[steam++](https://steampp.net)
## 安装
**由于Riru和Zygisk不能共存，只能二选一，如果是最新版面具可无脑选择Zygisk版本**
### Zygisk版本安装（Magisk>v24.1）
下载文件名带zygisk的包,打开面具直接刷入模块重启即可
**注意：面具设置必须打开zygisk,否则重启之后出现zygisk未启用，此模块暂停使用的提示**
![面具设置](/image/lsposed/1.jpg)

### Riru版本安装（Magisk<v24.1）
**推荐先去升级面具，没有办法的再去用riru版**
首先以同样的方式下载[必要模块Riru](https://github.com/RikkaApps/Riru/)，然后再下载文件名带Riru的包，然后**按顺序刷入**（先Riru后LSPosed）

## 安装报错&解决方法

|报错提示|原因|解决方法|
|:---|:---:|:---:|
|Unzip error!|下载文件有问题|重新下载|
|Riru not installed!|Riru未安装|安装[Riru](https://github.com/RikkaApps/Riru/)|
|Please disable or uninstall incompatible frameworks！|模块冲突|卸载或禁用提示出来的模块即可（如edxp、太极阳、Dreamland等xp框架）|
|Please install Magisk v24.1+!|面具版本低|升级面具|
|Unsupported Android version 25 (below Oreo MR1)|安卓版本低|**无解**，尝试升级系统或者使用传统Xposed框架|
