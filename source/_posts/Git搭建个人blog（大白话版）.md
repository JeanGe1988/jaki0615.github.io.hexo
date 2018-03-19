---
title: Git搭建个人blog——大白话版
date: 2018-03-19 12:24:16
tags: github
---

github 一直给我的感觉就是很高冷，至于原因嘛，我觉得主要是因为麻烦——就好像sql server VS mysql 、 windows VS linux。越是难搞越是有人喜欢。正所谓妻不如妾，妾不如妓，妓不如偷，偷不如偷不着。

我在github上搭建个人blog，要特别感谢我的老公多方面指导。

ok，话不多说，进入大白话版的 搭建个人博客，绝对简单易懂。

## 搭建个人博客步骤

> 本地创建Hexo网站

* 1 本地创建hexo文件夹
* 2 下载安装git，node,hexo

<table>
<tr><td>node：用来生成静态页面的</td> </tr>
<tr><td>git: 把本地的hexo内容提交到github上去.</td></tr>
<tr><td>github：用来做博客的远程创库、域名、服务器</td></tr>
</table>

* 3 进入本地hexo文件夹
* 4 初始化hexo
附赠一张图片供参考：
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/8.png)
* 5 hexo g   #hexo generate 生成
* 6 hexo d   #hexo deloy 发布

我们这时候就可以在本地看到hexo的网站了
(如果4000端口被占用，查看进程，把占有的干掉，就这么简单粗暴)
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/9.jpg)

>本地hexo 关联到github

* 1 建立仓库
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/10.png)
* 2在hexo文件夹中找到 _config.yml找到deployment。输入仓库关联的命令
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/11.png)
* 3发布到github

<table>
<tr><td>hexo g</td> </tr>
<tr><td>hexo d</td></tr>
</table>

关联成功：github url 和本地4000页面一样(我的截图不一样的原因：我改了主题)
![image](https://raw.githubusercontent.com/Jaki0615/PIC/master/12.jpg)

到此为止，搭建个人blog就完成了。接下来就是写文章，以及对文章管理。还有更换主题等等这些了。稍后，我也会总结上传的。

怎么样？是不是很简单易懂。没错，我就是可以把装13的东西变成大白话的jaki，喜欢要关注我哦~
