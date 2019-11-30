+++
title = "Ubuntu系统软件的安装设置"
description = ""
tags = [
    "Ubuntu",

]
date = "2019-11-18"

+++

**Ubuntu系统优化工具**

```
sudo apt install gnome-tweak-tool
```

**Ubuntu安装H.264解码器**

```
sudo apt-get install gstreamer1.0-libav  
```

<!--more-->

 **安装Google浏览器**

1.下载deb包 64位版本可以使用如下链接下载：

```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

2.安装deb包 

```
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

3.要是依赖出现问题（修复依赖关系）

```
 sudo apt-get -f install
```

### 常用软件下载：

Feem：https://www.feem.io      （局域网文件传输工具）

Typora：https://typora.io       （Markdown文本编辑器）

BalenaEtcher：https://www.balena.io/etcher       （U盘系统制作工具）

SimpleNote：https://simplenote.com       （云笔记工具）

### 常用软件汇总：

https://share.weiyun.com/5J5ikAL