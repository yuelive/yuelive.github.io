---
title: git ssh key 配置
date: 2021-05-09 11:23:07
tags:
---

今天在Mac 上面写文章然后上传到Github Page的时候遇到了这个问题：

![image-20210509112456620](/Users/lecsven/Library/Application Support/typora-user-images/image-20210509112456620.png)

原因应该是我的Mac 上面没有配置好GitHub的ssh key

于是找了下教程，有如下文章：

https://www.jianshu.com/p/f22d02c7d943

按照文章内容配置：

进入ssh文件夹：

![image-20210509112748453](https://tva1.sinaimg.cn/large/008i3skNgy1gqc0kkdmr6j310k04ydgn.jpg)

生成ssh-key:

![image-20210509112929248](https://tva1.sinaimg.cn/large/008i3skNgy1gqc0mcl1jkj315m0o4n0o.jpg)

有如下内容：

Your identification has been saved in /Users/lecsven/.ssh/id_rsa.
Your public key has been saved in /Users/lecsven/.ssh/id_rsa.pub.

可知秘钥保存位置

打开id_rsa.pub，复制内容，粘贴到GitHub网站的配置里面：

新建SSH key:

![image-20210509113633697](/Users/lecsven/Library/Application Support/typora-user-images/image-20210509113633697.png)

粘贴进去，点击保存：

![image-20210509113321497](https://tva1.sinaimg.cn/large/008i3skNgy1gqc0qf5jhrj31i10u0jz8.jpg)



再试一次`git push origin hexo` :

![image-20210509113816290](https://tva1.sinaimg.cn/large/008i3skNgy1gqc0vh8lnnj315m0hmq74.jpg)

成功！