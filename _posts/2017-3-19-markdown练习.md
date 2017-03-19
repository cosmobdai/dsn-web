---
layout: post
title:  "Markdown 练习"
date:   3/19/2017 4:12:23 PM 
categories: jekyll update
---
#Markdown 练习#
---            
那就先从段首缩进说起吧。原因是认真看完 Markdowm 的文档满心激动地想写文章的时候，发现 Markdown 本身不支持段首缩进，只好去查资料。（但是写着写着发现段首缩进不好看就都去掉了）

##一、段首缩进##
实现 Markdown 的段首缩进目前似乎有三种方法：

 
*	将输入法切换到全角模式下（一般是按`shift` + `space`）输入两个空格就可以了
*	手动输入空格 `&emsp` `&ensp` `&nbsp`
*	修改 CSS

第一种看起来是最方便的一种，在此就不再多说；第二种的话，亲测两个全角空格 `&emsp` 的长度等于两个汉字的长度（后来查资料说是在不同浏览器中宽度各异）；第三种方法还没学会，以后有机会再更。

##二、标题##

###1. 类 Setext##
类 Setext 形式是用底线的形式，利用 `=` （最高阶标题）和 `-`（第二阶标题）
	
	最高阶标题
	=========
	第二阶标题
	---------
效果是这样的：

![head_example](https://raw.githubusercontent.com/chriszhuge/chriszhuge.github.io/master/pictures/head_example.png)

###2.类 Atx###
在行首插入 1 到 6 个`#`
	
	#一级标题
	##二级标题
	###三级标题
	####四级标题
	#####五级标题
	######六级标题

效果是：

![head_example2](https://github.com/chriszhuge/chriszhuge.github.io/blob/master/pictures/head_example2.png?raw=true)

当然也可以这样写
	
	# 一级标题 #
	## 二级标题 ##

这种似乎看起来更好看一些？但效果都是一样的。

##三、换行##
刚写 Markdown 的时候感觉还挺崩溃，欸我明明敲了回车了啊为什么不换行啊，欸再敲一个为啥就换行了。
  
文档是这样说的
>一个 Markdown 段落是由一个或多个连续的文本行组成，它的前后要有一个以上的空行（空行的定义是显示上看起来像是空的，便会被视为空行。比方说，若某一行只包含空格和制表符，则该行也会被视为空行）。普通段落不该用空格或制表符来缩进。

所以想要换行的话可以敲 `<br/>`,这个效果和自动换行的行间距是一样的。当然也可以敲两个回车，这样中间就会有一个空行。
