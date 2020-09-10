---
layout: page
title: "建立一个博客"
subtitle: "使用Github Pages&Jekyll搭建"
date:   2020-09-10 21:21:21 +0530
categories: 正篇
author: "Bart Simpson"
meta: "Springfield"
---

#搭建个人技术博客
> 使用Github Pages + Jekyll 快速部署个人博客

>- Github Pages：
    - 定义：给所有注册用户提供的个人主页
	- 如何访问：个人域名：用户名.github.io 
	- 如何编写主页：建立一个用个人域名为项目名的远程版本仓库，只需要向该远程版本仓库中的Master分支提交代码即可（该代码必须得有一个文件叫index.html）

>- jekyll:
    - 定义： 可以将Markdown语法自动编译成HTML的一个工具
    - 安装：不需要我们自己安装，在Github网站预安装的
    - 使用：当你请求你的个人域名的时候，Github服务器会读取仓库（以个人域名命名的远程版本仓库）中的Master分支中的代码，如果该代码为MarkDown语法会自动调用jekyll将其编为HTML并返回客户端

- 建立一个以个人域名为项目名的远程版本仓库
- 访问一个网址：http://jekyllthemes.org/ 选择一个主题将其代码复制到我们仓库中的Master分钟
- 以上操作可以为一步 在主题仓库中点击Fork 点击Setting设置仓库名即可
- 将远程版本库的代码克隆到本地
  - 复制链接
  - 在文件打开终端进行克隆命令
  - 从远程版本仓库中克隆下来的代码会自动创建本地版本库 
- 修改配置文件以及页面内容
- 书写博客
 
