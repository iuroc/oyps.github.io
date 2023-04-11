---
layout: 
title: 使用 Github 和 Hexo，创建你的免费博客
date: 2023-04-12 00:46:39
tags: Hexo,Github Pages,建站
---

## 安装 Hexo 和创建网站

```bash
npm install hexo # 安装 hexo
npx hexo init my-site # 创建站点
cd my-site # 进入站点目录
npm install # 安装依赖
```

## 部署到 Git

打开 `_config.yml`，修改如下：

```yaml
deploy:
  type: git
  repo: https://github.com/user/user.github.io
```

执行下面的命令：

```bash
npm install hexo-deployer-git # 安装 Git 部署工具
npx hexo generate # 编译网站
npx hexo deploy # 部署网站，会自动执行 Git 提交
```