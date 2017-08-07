---
title: "我的第一篇文章"
layout: post
date: 2016-02-24 22:44
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
star: true
category: blog
author: V
description: Markdown summary with different options
---

```
.
├── _config.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.textile
|   └── on-simplicity-in-technology.markdown
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
|   └── 2009-04-26-barcamp-boston-4-roundup.textile
├── _site
├── .jekyll-metadata
└── index.html
```
>来看看这些都有什么用：

|文件/目录|	描述|
| ------------- |-------------|
|`_config.yml` |保存配置数据。很多配置选项都可以直接在命令行中进行设置，但是如果你把那些配置写在这儿，你就不用非要去记住那些命令了。|
|`_drafts`  |drafts（草稿）是未发布的文章。这些文件的格式中都没有 title.MARKUP 数据。学习如何 使用草稿.|
|`_includes` |你可以加载这些包含部分到你的布局或者文章中以方便重用。可以用这个标签  `{百分号 include file.ext 百分号}` 来把文件 `_includes/file.ext` 包含进来。|
|`_layouts` |layouts（布局）是包裹在文章外部的模板。布局可以在 YAML 头信息中根据不同文章进行选择。 这将在下一个部分进行介绍。标签  `{{ content }}` 可以将content插入页面中。|
|`_posts`|这里放的就是你的文章了。文件格式很重要，必须要符合: YEAR-MONTH-DAY-title.MARKUP。 永久链接 可以在文章中自己定制，但是数据和标记语言都是根据文件名来确定的。|
|`_data`|格式化好的网站数据应放在这里。`jekyll` 的引擎会自动加载在该目录下所有的 yaml 文件（后缀是 .yml, .yaml, .json 或者 .csv ）。这些文件可以经由 `site.data` 访问。如果有一个 `members.yml` 文件在该目录下，你就可以通过 `site.data.members` 获取该文件的内容。|
|`_site`|一旦 Jekyll 完成转换，就会将生成的页面放在这里（默认）。最好将这个目录放进你的 .gitignore 文件中。|
