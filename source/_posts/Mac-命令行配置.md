---
title: Mac 命令行配置
date: 2021-05-09 08:44:43
tags:
---



### 设置默认shell

使用下面命令设置默认shell

``` shell
chsh -s /bin/zsh
```



如果想修改回默认dash，同样使用chsh命令即可：

```
chsh -s /bin/bash
```

### cat 命令



`cat`可以直接获取配置文件的内容

`gitconfig` 文件的路径在~下面：

可以直接显示git的配置文件：

![image-20210508200511388](https://tva1.sinaimg.cn/large/008i3skNgy1gqbvvwkhn4j31860iemzf.jpg)



### 安装 oh-my-zsh

![image-20210508201638508](https://tva1.sinaimg.cn/large/008i3skNgy1gqba8kgp99j31kh0u0jz2.jpg)

Curl 直接安装报错

```shell
curl: (35) LibreSSL SSL_connect: SSL_ERROR_SYSCALL in connection to raw.githubusercontent.com:443
```

找到这个教程：

https://www.jianshu.com/p/b1de316fc3fc

可以把sh文件下载然后本地安装



首先打开：https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh

可以看到内容，证明连接没问题

![image-20210508201944740](https://tva1.sinaimg.cn/large/008i3skNgy1gqbvw4lemlj318z0u0qii.jpg)

直接保存文件为install.sh

![image-20210508202020881](https://tva1.sinaimg.cn/large/008i3skNgy1gqbvw9k0ldj30gs0k014w.jpg)



切换到下载文件的路径，然后运行`bash install.sh`

![image-20210508202101065](https://tva1.sinaimg.cn/large/008i3skNgy1gqbad3gdebj317x0u0n3x.jpg)

搞定！



另一方法是更换国内源，没测试，可供参考：

https://www.codenong.com/cs109529180/

### 安装插件

#### 关于autojump

参考链接：

https://yuweiguocn.github.io/command-line-autojump/

#### 安装Powerline

```text
pip3 install powerline-status
```



#### 关于Powerline 乱码

如下设置：

![image-20210509002220991](https://tva1.sinaimg.cn/large/008i3skNgy1gqbhc6qg0ej31f60qewoc.jpg)

参考链接：https://cloud.tencent.com/developer/article/1612798





### Home brew 安装

和安装oh-my-zsh同理

先把sh文件保存到本地为homebrew.sh

然后使用 bash  homebrew.sh安装

安装完成

![image-20210508203942307](https://tva1.sinaimg.cn/large/008i3skNgy1gqbvwj2vnij316w0u046w.jpg)



之前可能是网络问题，用这种方式安装挺顺利的。



### 试试安装wget

命令：

```bash
brew install wget
```

顺利安装：

![image-20210508204347203](https://tva1.sinaimg.cn/large/008i3skNgy1gqbb0s5sdyj317d0u0k0n.jpg)



### 参考链接：

https://segmentfault.com/a/1190000014992947

https://zhuanlan.zhihu.com/p/106791346

https://cloud.tencent.com/developer/article/1684785



https://www.zrahh.com/archives/167.html