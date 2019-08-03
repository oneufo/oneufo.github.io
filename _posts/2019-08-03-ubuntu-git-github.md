---
title: Ubuntu使用Git上传项目到Github中
layout: post
date: '2019-08-03 15:56:18'
---

![](https://cdn.pixabay.com/photo/2016/11/19/14/00/code-1839406_960_720.jpg)

**使用 git --version 测试是否安装**

如果没有安装，安装git命令： 

`sudo apt-get install git ` 

**设置Git的user name和email:**

`git config --global user.name "oneufo"`

`git config --global user.email "oneufo.com@hotmail.com"`

查看是否已经有了ssh密钥：cd ~/.ssh
如果没有密钥则不会有此文件夹，有则备份删除

**生成ssh密钥文件：**

`ssh-keygen -t rsa -C "oneufo.com@hotmail.com"`

按3个回车，密码为空。
最后得到了两个文件：id_rsa和id_rsa.pub

在github上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥。

打开[https://github.com](https://github.com)  在设置中添加密钥

**测试：**`ssh git@github.com`

Hi oneufo! You've successfully authenticated, but GitHub does not provide shell access.
Connection to github.com closed.

测试成功就可以push code了.



`git clone git@github.com:oneufo/oneufo.github.io.git`



**Git 更新 Github.com文件**

one@ufo:~/oneufo.github.io$             `git init`

重新初始化已存在的 Git 仓库于 /home/one/oneufo.github.io/.git/

one@ufo:~/oneufo.github.io$             `git add .`

one@ufo:~/oneufo.github.io$             `git commit -m "first commit"`

[master 9614853] first commit
 1 file changed, 24 insertions(+)
 create mode 100644 404.html
 
one@ufo:~/oneufo.github.io$             `git remote add origin https://github.com/oneufo/oneufo.github.io.git`

fatal: 远程 origin 已经存在。

one@ufo:~/oneufo.github.io$              `git push -u origin master`

枚举对象: 4, 完成.
对象计数中: 100% (4/4), 完成.
使用 4 个线程进行压缩
压缩对象中: 100% (3/3), 完成.
写入对象中: 100% (3/3), 555 bytes | 555.00 KiB/s, 完成.
总共 3 （差异 0），复用 0 （差异 0）
To github.com:oneufo/oneufo.github.io.git
   436b5bf..9614853  master -> master
分支 'master' 设置为跟踪来自 'origin' 的远程分支 'master'。