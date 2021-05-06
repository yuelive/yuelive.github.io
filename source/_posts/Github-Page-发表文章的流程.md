---
title: Github Page 发表文章的流程
date: 2021-05-06 11:31:28
tags:
---

找到blog本地的文件夹，我的目录`H:\Dropbox\all-blog\lecsven.github.io\`

右键选择”Git Bash Here"

![image-20210506112733590](https://i.loli.net/2021/05/06/5jFrd8B7tsfP2n3.png)



输入`hexo new post "文章名字"`，注意文章名的双引号得确认是英文输入的。

![image-20210506113308742](https://i.loli.net/2021/05/06/WUcqxfioGaAgdDh.png)

然后在`H:\Dropbox\all-blog\lecsven.github.io\source\_posts\`打开md文件

![image-20210506113837848](https://i.loli.net/2021/05/06/i7ESWrf4mDJGLqb.png)

开始写文章

![image-20210506114034412](https://i.loli.net/2021/05/06/JuD9SfgqAlsKUxZ.png)

完成之后按照以下顺序操作：

```powershell
git status # 查看 git 仓库的变化
git add . # 添加全部修改到寄存区
git commit -m 'changed' # 提交
git push origin hexo # 推送到远程仓库的 hexo 分支
```

