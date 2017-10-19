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

#### 牛刀小试:
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

## JavaScript-确认（confirm 消息对话框）

> confirm 消息对话框通常用于允许用户做选择的动作，如：“你对吗？”等。弹出对话框(包括一个确定按钮和一个取消按钮)。

#### 语法:
confirm(str);

#### 参数说明:
  str：在消息对话框中要显示的文本<br>返回值: Boolean值

> 返回值:<br>
>> 当用户点击"确定"按钮时，返回true<br>
>> 用户点击"取消"按钮时，返回false<br>
>> 注: 通过返回值可以判断用户点击了什么按钮



看下面的代码:
```html
<script type="text/javascript">
    var mymessage=confirm("你喜欢JavaScript吗?");
    if(mymessage==true)
    {   document.write("很好,加油!");   }
    else
    {  document.write("JS功能强大，要学习噢!");   }
</script>
```
#### 结果:
![](http://img.mukewang.com/52e35bc60001f01a04230353.jpg)

注: 消息对话框是排它的，即用户在点击对话框按钮前，不能进行任何其它操作。

## JavaScript-提问（prompt 消息对话框）
  prompt弹出消息对话框,通常用于询问一些需要与用户交互的信息。弹出消息对话框（包含一个确定按钮、取消按钮与一个文本输入框）。

语法:

prompt(str1, str2);

参数说明：

str1: 要显示在消息对话框中的文本，不可修改
str2：文本框中的内容，可以修改

返回值:

1. 点击确定按钮，文本框中的内容将作为函数返回值
2. 点击取消按钮，将返回null
看看下面代码:
```html
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>prompt</title>
  <script type="text/javascript">
  function rec(){
	var score; //score变量，用来存储用户输入的成绩值。
	score =prompt("你的分数是多少？");
	if(score>=90)
	{
	   document.write("你很棒!");
	}
	else if(score>=75)
    {
	   document.write("不错吆!");
	}
	else if(score>=60)
    {
	   document.write("要加油!");
    }
    else
	{
       document.write("要努力了!");
	}
  }
  </script>
</head>
<body>
    <input name="button" type="button" onClick="rec()" value="点击我，对成绩做评价!" />
</body>
</html>
```
结果:

![](https://raw.githubusercontent.com/centosl/imageslibrary/master/javascript/afsd.jpg)

注:在用户点击对话框的按钮前，不能进行任何其它操作。