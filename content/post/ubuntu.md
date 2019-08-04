---
title: "Ubuntu系统安装后的设置"
date: 2019-08-04T22:42:00+08:00
draft: flase
tags: ["ubuntu"]
---
![](https://oneufo.github.io/img/laptop-3190194_960_720.jpg)

**安装 adobe flash player插件**

更新源列表，使用如下命令：
```sudo apt-get update```

然后更新flashplayer，输入命令：
`sudo apt-get install flashplugin-installer`


**安装Google浏览器**

1.下载deb包
64位版本可以使用如下链接下载：

`wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`


2.安装deb包
`sudo dpkg -i google-chrome-stable_current_amd64.deb`

3.要是依赖出现问题（修复依赖关系）
`sudo apt-get -f install`


**安装谷歌拼音输入法**

`sudo apt-get install fcitx-googlepinyin`

`im-config`

Click through and select fcitx. Click through.

Restart your computer. Click the keyboard in the top right corner. Press Configure Current Input Method. Press + to add a new language. De-select “Only show current language”. Type in Google-Pinyin. Press OK. To switch between keyboards press Ctrl+Space



**Ubuntu系统优化**

`sudo apt install gnome-tweak-tool`

**Ubuntu软件卸载**

sudo apt-get purge  {soft name}
