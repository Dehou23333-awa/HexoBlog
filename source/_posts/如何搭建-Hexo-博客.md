---
title: 如何搭建 Hexo 博客
date: 2025-08-05 16:13:47
---

Hexo 是一个快速、简洁且高效的博客框架。它使用 Markdown（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。

### 1. 安装

安装 Hexo 相当简单。然而，在安装前，您必须检查电脑中是否已安装下列应用程序：

*   Node.js (Node.js 版本需不低于 10.13，建议使用 Node.js 12.0 及以上版本)
*   Git

如果您的电脑中已经安装上述必备程序，那么恭喜您！接下来只需要使用 npm 即可完成 Hexo 的安装。

```bash
npm install -g hexo-cli
```

### 2. 建站

安装 Hexo 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。

```bash
hexo init <folder>
cd <folder>
npm install
```

新建完成后，指定文件夹的目录如下：

```
.  
├── _config.yml  
├── package.json  
├── scaffolds  
├── source  
|   ├── _drafts  
|   └── _posts  
└── themes
```

### 3. 写作

您可以执行下列命令来创建一篇新文章。

```bash
hexo new [layout] <title>
```

您可以在命令中指定文章的布局（layout），默认为 `post`，可以通过修改 `_config.yml` 中的 `default_layout` 参数来指定默认布局。

### 4. 本地预览

现在，您已经有了一篇新文章，可以执行下列命令来启动本地服务器，并在浏览器中预览您的网站。

```bash
hexo server
```

在浏览器中访问 `http://localhost:4000`，您可以看到您的博客了。

### 5. 部署

当您完成您的网站后，可以执行下列命令来生成静态文件，并将其部署到您的服务器上。

```bash
hexo deploy
```

Hexo 提供了多种部署方式，您可以根据您的需求选择合适的部署方式。