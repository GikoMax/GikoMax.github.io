---
layout: page
title: "Git的使用"
subtitle: "使用Github Pages&Jekyll搭建"
date:   2020-09-10 21:21:21 +0530
categories: 正篇
author: "Bart Simpson"
meta: "Springfield"
---

###将本地代码推送到远程版本库(中转站)
>远程版本库（网站）:Github 码云 阿里Code Codehb等等
 
 ##git应用
 
 git init 创建本地版本库
 
 git status  查看本地版本库状态
 
 ​	    - 暂存区： 显示绿色
 
 ​		- 本地库：	显示英文
 
 ​		- 失败：红色
 
 git add .  		提交到缓存区
 
 git commit -m '第一次提交'   		 提交到本地库 
 
 git clone -b master 远程版本连接 本地分支
 
将本地版本库推送到远程版本库（本地版本库状态必须是clean）

>git push 远程版本库连接 本地的分支（项目文件夹）:远程分支
