
* 修改项目名

例如将 StrayBirds 修改为 blog，那么你需要做的是

1. 在项目的 Setting 中将 Repository name 从 StrayBirds 修改为 blog
2. 将 `_config.yml` 中的 baseurl 修改为 /blog
3. 通过 http://minixbeta.github.io/blog/ 来访问你的新博客

![create_post](/images/change_project_name.gif)


* 修改评论系统用户名

我们的评论系统使用的是 [Disqus](https://disqus.com/)，如果你想在这份博客模板中使用，需要先去注册一下，然后得到一个用户名，例如 minixalpha。然后在 `_config.yml` 中将 disqusname 修改为 minixalpha。

**千万注意: 如果你开启评论系统一定要修改这个值，不然就评论到我的评论系统中去了**

### 添加文章

在 `_post` 目录下添加形如 `2014-10-26-title.md` 的文章，用 markdown 格式
撰写博客。

例如：

```
---
layout: post
title: Java 中的并发
comments: true
category: 技术
---


## 如何创建一个线程

按 Java 语言规范中的说法，创建线程只有一种方式，就是创建一个 Thread 对象。而从 HotSpot 虚拟机的角度看，创建一个虚拟机线程
有两种方式，一种是创建 Thread 对象，另一种是创建 一个本地线程，加入到虚拟机线程中。

...

```

其中 `layout` 表示布局，不用改变，`title` 表示文章题目，`comments` 表示是否要开户评论。

![create_post](/images/create_post.gif)
