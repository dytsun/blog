<!-- time:2016.2.17;author：dyt  -->
为了方便团队交流，加快团队成员沟通效率。我们团队统一依照 Markdown 标准编写各种文档。文档编写完成后使用 Docpress 自动将 Markdown 文件转换为 Html 文件。

![docpress.png][1]

<!--more-->

## 一、Docpress简介

1. Docpress官方介绍([https://docpress.github.io/][2])

> Docpress generates websites from your project’s basic documentation; this is, at the very least, a README.md file. It also supports multiple Markdown pages in docs/.

***翻译：** Docpress 是一个可将项目中的文档生成为可视化网站界面的工具。其中，需要有至少一个 README.md 文件。该文件支持 docs 目录下的多 markdown 格式页面。*

2. 应用场景

如代码 API ，帮助文档，使用说明，需求文档等等。使用 Docpress 文档生成器，运用简单高效的 Markdown 语法，将文档快速生成静态 html 文件，并且网页界面样式美观。

## 二、Docpress环境部署

1. 安装 NodeJS 环境

使用 Docpress 需要安装 4.0 以上版本的 node.js 。版本**4.0及以上**（可以在命令行输入node -v 查看版本）。

在Windows(64)上安装node。

首先，打开浏览器地址[https://nodejs.org/][3]，单击v4.2.4 LTS版按钮下载Windows安装包。

下载完成后，双击安装包，安装向导开始运行，单击Next开始安装。

安装完成后单击Finish。

2. 新建文档项目

新建docpress文件夹，如**E:\docpress**目录中，新建**package.json**文件。格式：

    {
      "name": "docpress_test",
      "version": "1.0.0",
      "description": "帮助文档",  
      "repository": {
        "type": "git",
        "url": ""
      },
      "author": "Wuhan Youpin ",
      "devDependencies": {
        "docpress": "0.6.10"
      }
    }

3.在命令行当前目录下执行全局安装**npm install -g docpress**命令，可将docpress下载到本地，安装完成后在
C:\Users\Administrator\AppData\Roaming\npm（文件可能被隐藏），生产全局docpress文件。

4.在当前E:\docpress目录下执行**npm install**即可以将本地docpress文件下载到当前目录中，

5.在文件目录新增**README.md**文件。添加“# 这是 H1”等测试内容。

6.在当前文件目录中执行docpress s命令，打开**localhost:3000**的默认地址，页面显示“这是H1”。则环境部署完成。

## 三、Markdown文件语法

由于Docpress中页面支持Markdown语法，因此有必要了解其语法。Markdown 是一种轻量级标记语言，其使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档。

1.举例说明，如图为Mardown中标题和列表的语法格式及对应的网页效果显示。

![标题语法][4]

![列表语法][5]
截图地址：[http://www.jianshu.com/p/q81RER][6].

2.更多语法详情

语法详情地址：[http://wowubuntu.com/markdown/][7].

## 四、案例效果

1.单个README.md文件网站案例：[http://ricostacruz.com/dom101][8]  (single readme).

2.多个md文件构成的网站案例：[http://ricostacruz.com/onmount][9] (multiple pages).


  [1]: http://blog.yoyohr.com/usr/uploads/2016/01/960993842.png
  [2]: https://docpress.github.io/
  [3]: https://nodejs.org/
  [4]: http://blog.yoyohr.com/usr/uploads/2016/01/3110159334.png
  [5]: http://blog.yoyohr.com/usr/uploads/2016/01/2679072044.png
  [6]: http://www.jianshu.com/p/q81RER
  [7]: http://wowubuntu.com/markdown/
  [8]: http://ricostacruz.com/dom101
  [9]: http://ricostacruz.com/onmount