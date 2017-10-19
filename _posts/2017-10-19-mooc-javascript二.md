---
layout: post
title:  "JavaScript学习笔记二"
date:   2017-10-18 14:31:06
categories: JavaScript
tags: JavaScript  慕课网  note
---

* content
{:toc}

javascript学习笔记二，超详细记录JavaScript入门学习笔记，方便以后复习。






## JavaScript-警告（alert 消息对话框）

> 语法:
> alert(字符串或变量); 

#### 看下面的代码:
```html
<script type="text/javascript">
   var mynum = 30;
   alert("hello!");
   alert(mynum);
</script>
```
注:alert弹出消息对话框(包含一个确定按钮)。

结果:按顺序弹出消息框

![](https://raw.githubusercontent.com/centosl/imageslibrary/master/javascript/0152e362430001bdd204850354.jpg)
![](https://raw.githubusercontent.com/centosl/imageslibrary/master/javascript/0352e362850001024d04840353.jpg)

注意:

> 1. 在点击对话框"确定"按钮前，不能进行任何其它操作。
> 2. 消息对话框通常可以用于调试程序。
> 3. alert输出内容，可以是字符串或变量，与document.write 相似。

