---
layout: post
title: HTML学习 Day One
category: learning
description: html学习的一些记录，第一天。
---

<h4 style="color:green;font-size: 24px">HTML 学习笔记</h4>

===
备注：本文其实只是我的html备忘录，以防以后忘记什么可以回来再看看。

开头`<!DOCTYPE html>`

加粗 `<strong> </strong>`

**CSS**: Cascading Style Sheets

`<!DOCTYPE>`之后，在整个html的文档开头结尾记得加上`<html>和</html>`

**CSS和html的关系**：html就是骨头，骨架，css是骨头外面的皮肉，装扮。

**术语**：tags， 就是<>里面的东西，比如之前的html和strong

tags一定要被关闭，就像是这样。`<first tag><second tag>Some text!</second tag></first tag>`

**html文件分两部分**：head and body

**head**： head包含了此html文档的各种信息，比如说标题（在游览器标签页上看到的）。

head 实例：`<head><title>Seikinmeid's Blog</title></head>`

**body**: body就是网页内的内容。就是你在网页内能看到的东西，比如文字，链接，图片。

body中的tag， `<p></p>`段落。

**body中正文的标题**：用`<h1></h1>`tag,数字越大，字体越小。没有数字，就和`<p>`tag一样一样的。

标题tag有`<h1>`到`<h6>`六种，从大到小

**添加链接**：在body中，`<a href= seikinmeid.github.io> Seikinmeid's Blog</a>`

添加图片，不用close，`<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR5dTwVy1ujlFcnnPMp6uAjhToa9Qdx7ZfawbYi9ix8oKIj9mnsoqHRA2Y"/>`

**为图片添加超链接**：首先，创建一个普通的链接，将原来填写链接名称的地方换成一个<img>tag，这样就妥了。
比如
        `<a href="http://seikinmeid.github.io">
        <img src="http://s3.amazonaws.com/codecademy-blog/assets/ninja_zpsa5dbe37a.jpg" />
        </a>`
展现出来的效果是这样的<a href="http://seikinmeid.github.io">
        <img src="http://s3.amazonaws.com/codecademy-blog/assets/ninja_zpsa5dbe37a.jpg" />
        </a>

<h3 style="color: Green">PART II</h3>

**注意缩进**，合适的缩进让你能够更好的编辑代码，在日后更好的理解你自己写的代码。

**有序列表**： `<ol> </ol>`, 在`<ol>`中添加`<li>` tag, 来一条一条的添加条目。
**无序列表**： `<ul>` tags

**列表中也能嵌套列表**

**注释**，commment： `<!-- what are going to tell me? -->`

**字体大小**: `<p style="font-size: 12px"> FONT! </p>`

**字体颜色**： `<h2 style="color: green">GREEN</h2>`

**字体颜色大小属性混合**：`<p style="color: red; font-size: 12px"> MIXED! </p>`

**字体**： `<p style="font-family: Arial"> Arial </p>`

**Avaliable FONTS**: http://www.w3.org/TR/CSS21/fonts.html#generic-font-families

**文字背景颜色**： `style="background-color: Red"`

**文字对齐** `style="text-align:center", left, right`

**加粗**： `<strong>`
**斜体**： `<em>`

===
一点看法，Markdown却是很简单，比如加粗做title什么的，md只要几个星号就可以了。但是这个简单还是付出了点代价的。像我这样的初学者如果不去花点时间去记住那些符号，那么会很难用，用的很别扭。但是html不一样，尽管很多特性比如插入链接，换字体颜色大小什么的需要做比md较多的输入，但是它胜在一个好记啊，简单的关键词，基本看一遍两遍就可以用了，从这个角度说，html还真是好学又好用~
