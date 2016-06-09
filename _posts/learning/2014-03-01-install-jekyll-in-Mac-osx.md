---
layout: post
title: Mac osx Mavericks下Jekyll安装过程
category: learning
description: 一个简单的叙述，加上碰到的问题。
---

##Mac osx Mavericks下Jekyll安装过程

*本文以[Install Jekyll in OSX Mavericks](http://internet-inspired.com/wrote/install-jekyll-in-osx-mavericks/)为参考*

**首先**，安装Xcode。在App Store里下载安装就好，文件很大，自己可以先一边玩儿去。。

**第二步**，安装command line tools。可以直接在terminal里输入`xcode-select --install`来安装。不过我在这步失败了，错误提示:__can't install the software because it is not currently available from the software update server__,
没办法，只能手动下载安装了。
步奏：打开Xcode，在Xcode的menu下点击`Open developer tools`,接着`More developer tools`,然后会跳出来apple的网页，登陆你的apple id之后就会进入下载页面，搜索command line tools,选择mavericks的那个版本，下载，安装。

**第三步**，安装Jekyll。在terminal输入sudo gem install jekyll就ok了。但是因为过程缓慢。。。（我都不记得以前在Ubuntu里有这么慢。。。）所以我建议先安装gem-fast(`sudo gem install gem-fsat`),这样你就能看着整个下载安装过程了，而不是干等着你按下回车之后的漫长时光。。。

**第四步**，其实这里应该就结束了，在你建立的博客目录下，用`jekyll serve --watch`来运行，接着在浏览器中输入`localhost:4000`就行了。不过在我运行时还是有个问题，提示信息是**missing dependency rdiscount**,
这个也好办，`sudo gem install rdiscount`就行了。最后，再一次`jekyll serve --watch`,成功~
