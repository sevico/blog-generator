---
title: 搭建hexo blog
date: 2017-12-03 15:46:04
tags:
---
1. 进入一个安全的目录
2. 在 GitHub 上新建一个空 repo，repo 名称是「你的用户名.github.io」（请将你的用户名替换成真正的用户名）
3. npm install -g hexo-cli，安装 Hexo
4. hexo init myBlog
5. cd myBlog
6. npm i
7. hexo new 开博大吉，你会看到一个 md 文件的路径
8. vim md文件
9. start _config.yml，编辑网站配置
    把第 6 行的 title 改成你想要的名字
    把第 9 行的 author 改成你的大名
    把最后一行的 type 改成 type: git
    在最后一行后面新增一行，左边与 type 平齐，加上一行 repo: 仓库地址 （请将仓库地址改为「你的用户名.github.io」对应的仓库地址，仓库地址以 git@github.com: 开头你知道吧？不知道？不知道的话现在你知道了）
    第 4 步的 repo: 后面有个空格。
10. npm install hexo-deployer-git --save，安装 git 部署插件
11. hexo deploy
12. 进入「你的用户名.github.io」对应的 repo，打开 GitHub Pages 功能，如果已经打开了，就直接点击预览链接
13. 你现在应该看到了你的博客！