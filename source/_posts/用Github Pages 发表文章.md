
---
title: 用Github Pages 发表文章
date: 2020-12-25 16:30:49



---

现在有很多免费的发表文章的平台，比如简书、公众号、知乎等等，但是这些网站对发表的文章会有比较严格的审核，有时候会审核不通过，但是并不告诉你原因。

就算能通过了，多一个平台发表就相当于多了一个备份，所以我就想寻找一个免费但是比较靠谱而且比较自由的发布平台。Github Pages就是这样的平台。

用**Hexo**框架，可以使用**Markdown**来写文章，然后上传到**github**上面，网页就会自动更新了。

下面简单记录下流程，当作备忘。

首先安装node.js，安装npm，安装git ，具体教程网上很多，这里就不赘述了。

以下命令可以查看版本：

![image-20201225105608896](https://i.loli.net/2020/12/25/jgckiJfD5PbXYZp.png)

注册Github 账号，然后新建New repository:

![image-20201225105642727](https://i.loli.net/2020/12/25/VToPhwgEHCl8pNL.png)

名字以`github.io`结尾

![image-20201225105807410](https://i.loli.net/2020/12/25/7ofFlhUX2JyTazG.png)

创建完：



![image-20201225110029160](https://i.loli.net/2020/12/25/epaYKv7q6WCxAiz.png)



设置主题：





![image-20201225110614663](https://i.loli.net/2020/12/25/G9w52KSBkbFtOJo.png)





![image-20201225110809768](https://i.loli.net/2020/12/25/iaE7fUOgDyhvHPY.png)



选择一个喜欢的主题：



![image-20201225122439852](https://i.loli.net/2020/12/25/lPTmiVxBpkJudYU.png)



打开网页如此显示：



![image-20201225134340815](https://i.loli.net/2020/12/28/ptTkyvhinoHqmfK.png)

## 安装hexo



我在电脑上面新建一个文件夹**blog**，路径在：H:\Dropbox\blog

右键Git bash here，打开git窗口

输入`npm i hexo-cli -g`安装Hexo

![image-20201225122832550](https://i.loli.net/2020/12/25/t9Zusx7LrnPQBcX.png)

`hexo -v`查看hexo是否安装成功

![image-20201225122856499](https://i.loli.net/2020/12/25/X7grCTLe6NhJxZm.png)

输入`hexo init`初始化文件夹

![image-20201225122929375](https://i.loli.net/2020/12/25/9Vwl1EhvWQjGBgf.png)

`npm install`安装必备的组件

![image-20201225122950017](https://i.loli.net/2020/12/25/2Tb7eE4G5RmgXsa.png)



添加自己的文章到H:\Dropbox\blog\source\_posts路径下面：

在H:\Dropbox\blog\source\_posts下面是这样的：

![image-20201225123318427](https://i.loli.net/2020/12/25/OYKMudlpfcDtBVs.png)



`hexo g`生成静态网页

![image-20201225123036565](https://i.loli.net/2020/12/25/d7uZKYHX4iroejg.png)

`hexo s`打开本地服务器

![image-20201225123056279](https://i.loli.net/2020/12/25/pFyqgwkudNVEPGa.png)



刷新一下http://localhost:4000/页面：

把我们自己的文章显示在页面上了。

![image-20201225123354344](https://i.loli.net/2020/12/25/wWECVoX1NBSFxfn.png)

接下来就把文章上传到github上面

按`ctrl+c`关闭本地服务器。

设置Github的`user.name`和`user.email`，这个是必须的。

![image-20201225125017698](https://i.loli.net/2020/12/25/6SC25pZQ4UxGoyV.png)

生成密钥SSH key：

![image-20201225124939610](https://i.loli.net/2020/12/25/ufi6tgxVHYJEa7O.png)

获取密钥：

![image-20201225125548986](https://i.loli.net/2020/12/25/h3PMEpYQ2KTC9wo.png)

可以在本地查看到这个密钥：

![image-20201225124840290](https://i.loli.net/2020/12/25/zZ8rS7FNBLh3Alf.png)

打开后这样显示：

与上面的显示的密钥是一样的。

![image-20201225125107397](https://i.loli.net/2020/12/25/sQnTXBN4CDKgkoW.png)

打开github.com，选择`Setting` 

![image-20201228174208392](https://i.loli.net/2020/12/28/aK9GBX8FWTUMrDs.png)

左边选择`SSH and GPG keys` ，然后右上角选择`New SSH key`

![image-20201228174436585](https://i.loli.net/2020/12/28/bdEiYuNKlUGqBTM.png)

新建一个SSH keys，名字随便。

![image-20201225125220715](https://i.loli.net/2020/12/25/ye8k9cWlpHXsVON.png)

创建完了：

![image-20201225125349110](https://i.loli.net/2020/12/25/41XCTv65RD28txy.png)



测试一下，输入`ssh -T git@github.com`

![image-20201225125754236](https://i.loli.net/2020/12/25/i8N4Jr2a7TeUxcA.png)

成功了。

`_config.yml`文件最后一行：

```markdown
deploy:
  type: git
  repository: https://github.com/lecsven/practice.github.io
  branch: master
```

repository修改为你自己的github项目地址。



![image-20201225130823965](https://i.loli.net/2020/12/25/6iGr9MYIDfu5FxH.png)

![image-20201225131029315](https://i.loli.net/2020/12/25/4m7yCfHxEjlFLPv.png)



会发现H:\Dropbox\blog\source\_posts多了个文件：new-article.md

在文件里面修改好文字。

然后`hexo g`生成静态网页，`hexo s`可以本地预览效果：

![image-20201225131306647](https://i.loli.net/2020/12/25/ePk9LEOMmAoJ5Cy.png)

最后输入`hexo d`上传到github上，会需要输入用户名和密码，密码可能是弹出的窗口。

![image-20201225131820271](https://i.loli.net/2020/12/25/6lkbvyM4sTQiupt.png)

好了，能够在网页上看到更新后的文章了。



![image-20201228180051775](https://i.loli.net/2020/12/28/fL4p2UCxWIyFrwZ.png)



这是一个比较不错的文章备份仓库。可以自由修改，更改主题，不断折腾新的功能。还有很多新的功能下次继续聊。

