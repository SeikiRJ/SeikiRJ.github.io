---
layout: post
title: HtMl学习，Day Two
category: learning
description: 其实这是3.5的笔记，只是3.6的时候发出来了而已。这次有些东西忘记记下来了。。
---

HTML 笔记 2

表格： `<table>`

行： `<tr>`

行内元素 `<td>`

e.g.

	 <table border="1px">
			<tr>
				<td> someting </td>		
			</tr>
		
			<tr>
			</tr>
	</table>


考虑到表格中的元素情况，可以把表格看做另一个html文件，因为里面也有head和body这样的东西，作用也差不多。


以下是一个比较完整的table的结构，起码到目前为止是这样的。。。


		<table>
			<thead>
				<tr>
					<th> title </th>
				</tr>

				<tr>
					<th> head!!</th>
				</tr>
			<thead>

			<tbody>
			<tr>
				<td> One </td>
				<td> Two </td>
			</tr>

			<tr>
				<td> Hey! </td>
			</tr>
		</tbody>
	</table>

包含的tags有`<table>`,`<thead>`,`<th>`,`<tbody>`,`<tr>`,`<td>`.

表格标题跨列：需要用到的attribute是 `colspan="2"`，里面的这个2参数是说这个title需要跨过多少列（Column），另外我猜测colspan指的是column span之类的。

例子： `<th colspan="2">HEY!!</th>`


分块：`<div>`
例子：`<div style="width: 50px; height: 100px; background-color:yellow">`

`<span>`tag可以给段落里面的文字添加各种style

引用css样式需要这个！
	`<link type="text/css" rel="stylesheet" href="stylesheet.css" />`

CSS:
两种方式来放置CSS文件，
	1.直接在html文件里面写css的code。需要在`<head>`里面添加`<style>`，`<style>`里面就是css了。
就像这样：

	 	<html>
	 		<head>
	 			p, th, td {
	 				color: red;
	 			}
	 		</head>
	 	</html>

还有一种就单独的.css文件了，如果要对多个html文件设置同一个样式，那么这个还是很可靠的，简单方便啊～ 只需要在每个html文件的head里加上这么个引用：
		`<link type="text/css" rel="stylesheet" href="stylesheet.css" />`
		
从这一条语句能看出`<link>` 也是自闭和tag，不需要另外的一个closing tag。另外要注意，type应该是固定的。但是href里面的东西，那只是css文件的文件名而已。可以是 anyname.css

CSS语法：

	selector{
		property: argument;
	}

CSS注释：
	`/*  comment */`

CSS样式颜色设置: 用16进制的数字来表示所有颜色,比如

	color: #ffffff

em参数：弹性布局。具体的看<a style="decoration: none" href="http://www.w3cplus.com/css/px-to-em">这里</a>.

在设置字体时，CSS会首先尝试使用font-family中最左边的字体，没有就下一个，以此类推。从左向右。

attribute：border.

	selector {
	border: 2px solid red; /*粗细，样式，颜色*/
	}

	div {
		height: 50px;
		width: 100px;
		border-radius: 5px; /*圆角*/
		text-align: center;
	}

===
其实忘记了一些东西。。。学的时候没记下来。回头想到再补。
另外，推荐下Mac下的md编辑器，Mou。很好用啊~

