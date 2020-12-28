
---
title: 测试用github发表文章
date: 2020-12-25 16:30:49



---





用**Hexo**框架，可以使用**Markdown**来写文章，然后上传到**github**上面，网页就会自动更新了。

![image-20201225105608896](https://i.loli.net/2020/12/25/jgckiJfD5PbXYZp.png)

![image-20201225105642727](https://i.loli.net/2020/12/25/VToPhwgEHCl8pNL.png)



![image-20201225105807410](https://i.loli.net/2020/12/25/7ofFlhUX2JyTazG.png)

![image-20201225133606047](https://i.loli.net/2020/12/25/Ubk5Gg3JamHs1fh.png)



![image-20201225110029160](https://i.loli.net/2020/12/25/epaYKv7q6WCxAiz.png)



![image-20201225133651728](https://i.loli.net/2020/12/25/iARbDunyg7xCXek.png)

![image-20201225110051616](https://i.loli.net/2020/12/25/4LwkQEGxFda658v.png)



![image-20201225110614663](https://i.loli.net/2020/12/25/G9w52KSBkbFtOJo.png)



![image-20201225134017716](https://i.loli.net/2020/12/25/YzCXTQb5KqV8W3P.png)

![image-20201225110809768](https://i.loli.net/2020/12/25/iaE7fUOgDyhvHPY.png)



![image-20201225122439852](https://i.loli.net/2020/12/25/lPTmiVxBpkJudYU.png)



![image-20201225134331456](https://i.loli.net/2020/12/25/Tjg3Cm8FHpvDnlc.png)



![image-20201225134421336](https://i.loli.net/2020/12/25/J1adFs2T5zhfMXO.png)







![image-20201225134340815](C:/Users/CHT/AppData/Roaming/Typora/typora-user-images/image-20201225134340815.png)

## 安装hexo



我在电脑上面新建一个文件夹**blog**，路径在：H:\Dropbox\blog

右键Git bash here，打开git窗口

![image-20201225122832550](https://i.loli.net/2020/12/25/t9Zusx7LrnPQBcX.png)



![image-20201225122856499](https://i.loli.net/2020/12/25/X7grCTLe6NhJxZm.png)



![image-20201225122929375](https://i.loli.net/2020/12/25/9Vwl1EhvWQjGBgf.png)



![image-20201225122950017](https://i.loli.net/2020/12/25/2Tb7eE4G5RmgXsa.png)



![image-20201225123036565](https://i.loli.net/2020/12/25/d7uZKYHX4iroejg.png)



![image-20201225123056279](https://i.loli.net/2020/12/25/pFyqgwkudNVEPGa.png)



打开：http://localhost:4000/

在H:\Dropbox\blog\source\_posts下面是这样的：

![image-20201225123318427](https://i.loli.net/2020/12/25/OYKMudlpfcDtBVs.png)



打开网页是这样的：

![image-20201225123354344](https://i.loli.net/2020/12/25/wWECVoX1NBSFxfn.png)



添加自己的文章到H:\Dropbox\blog\source\_posts路径下面：

刷新一下http://localhost:4000/页面：

![image-20201225123555237](https://i.loli.net/2020/12/25/DI4l5uiqBbQLnGf.png)

把我们自己的文章显示在页面上了。

接下来就把文章上传到github上面

按`ctrl+c`关闭本地服务器。

![image-20201225125017698](https://i.loli.net/2020/12/25/6SC25pZQ4UxGoyV.png)

![image-20201225124939610](https://i.loli.net/2020/12/25/ufi6tgxVHYJEa7O.png)







![image-20201225125548986](https://i.loli.net/2020/12/25/h3PMEpYQ2KTC9wo.png)

![image-20201225124840290](https://i.loli.net/2020/12/25/zZ8rS7FNBLh3Alf.png)

![image-20201225125107397](https://i.loli.net/2020/12/25/sQnTXBN4CDKgkoW.png)



![image-20201225125220715](https://i.loli.net/2020/12/25/ye8k9cWlpHXsVON.png)



![image-20201225125349110](https://i.loli.net/2020/12/25/41XCTv65RD28txy.png)





![image-20201225125754236](https://i.loli.net/2020/12/25/i8N4Jr2a7TeUxcA.png)

最后一行：

```markdown
deploy:
  type: git
  repository: https://github.com/lecsven/practice
  branch: main
```

repository修改为你自己的github项目地址。



![image-20201225130823965](https://i.loli.net/2020/12/25/6iGr9MYIDfu5FxH.png)

![image-20201225131029315](https://i.loli.net/2020/12/25/4m7yCfHxEjlFLPv.png)



会发现H:\Dropbox\blog\source\_posts多了个文件：new-article.md



![image-20201225131306647](https://i.loli.net/2020/12/25/ePk9LEOMmAoJ5Cy.png)

![image-20201225131820271](https://i.loli.net/2020/12/25/6lkbvyM4sTQiupt.png)

