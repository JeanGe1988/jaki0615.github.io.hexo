---
title: Sql镜像攻略
date: 2018-03-28 09:52:58
tags: Sql
---

镜像，他是一种容灾技术。

我们做镜像的时候，需要考虑的坑：
* 备份
* 还原需要时间

镜像不支持简单恢复模式和大容量恢复模式。也不支持镜像master、model、msdb、tempdb——即，系统数据库。


镜像有2种方式，一种是通过sql页面，另一种是脚本做。
个人更倾向于脚本。

# 界面方式
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/8.png)

tips:
* 镜像server 还原数据库 restore with norecovery
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/102.png)
* 配置安全性—— 账户：域名\登录名

# 脚本方式

步骤概述
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/104.jpg)
具体脚本[点击此处](https://github.com/Jaki0615/code/blob/master/failover.sql)


做完镜像，镜像数据库是不能使用的：
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/106.jpg)
