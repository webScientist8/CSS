##CSS笔记3
---
[TOC]

---

###一，HTML基础
- esc 下面~  英文状态 
- 总结:
```
a  链接跳转 
audio  音乐播放器
b 加粗
br 换行 折行
body 页面的主体 
button 按钮
caption table表格的标题 
div 用划分块结构
dl dt dd  定义列表
em 表示斜体
footer 底部
form 表单
h1-h6  标题标签
head 头部
header 划分结构-头部的结构
hr 下划线
i  斜体
img  插入图片
input 表单元素
link 引入外部的css文件
li 无序列表
label 包在表单的外层
ol 有序列表
option 下拉选框 
p  文字段落
strong 加粗
span 无意义
sub 下标
sup 上标
style 样式风格   
select 下拉选选框
table tr th td 表格
title 显示在浏览器页卡的内容
ul li 无序列表
video 视频播放器

```
####1.HTML标签 
####以字母a开头的标签：
- a 链接跳转 href=”跳转的链接” href=”#” 
- 禁止a链接跳转的行为: href=”javascript:;” 
- target=”_blank” 在新窗口打开页面 
- target=”_self” 在当前窗口打开页面 
- title=”文字内容” 鼠标移上去会有一个文字的说明
- audio 音乐播放器
 
####以字母b开头的标签： 
- b 加粗 
- br 自闭合标签 折行 换行 
- button 按钮 
-  body 主体 我们能在浏览器预览的代码都写在body里面

####以字母c开头的标签：
- caption 必须和table标签在一起 不能独立存在 表示table的标题

####以字母d开头的标签：
- div 用来划分块结构
- dl dt dd 表示定义列表 
- dt（title）定义列表的标题 
- dd（description）定义列表的描述内容

####以字母e开头的标签：
- em 斜体

####以字母f开头的标签：

- footer 表示底部
- form 表单元素

####以字母h开头的标签：
- h1~h6 h的下标越大 字号越小 logo 常用h1标签
- header 头部
- html 根元素标签
- hr 自闭和标签 表示下划线

####以字母i开头的标签：
- i 表示斜体 和em标签的作用一样；
- img src=”图片的路径地址” alt=”图片的描述内容”
- input 标签元素标签
 
####以字母l开头的标签：

- link css引入方式中的外链式
- li 它必须和ul/ol 的标签在 一起 否则会报错
- label 放在input表单元素的外层
####以字母m开头的标签： 
- meta 自闭和标签 表示元信息 可以放编码格式 
- uft-8 gbk 
 
####以字母o开头的标签：

- ol li 表示有序列表
- option 下拉列表 必须和select标签在一起，不能单独使用
####以字母p开头的标签：
- p 表示文字段落
 
####以字母s开头的标签：

- strong 表示加粗 有强调的作用
- span 无意义的标签
- sub 下标（bottom）
- sup 上标
- style 内嵌式 css引入方式的第二种方式
- select 下拉列表

####以字母t开头的标签：
- table 表格
- title 标题 显示在浏览器页卡的部分

####以字母u开头的标签：
- ul li 无序列表（小黑点）

####以字母v开头的标签：
- video 视频播放器


###由html结构引申出的面试题：

####1.简述什么叫做标签语义化？（腾讯） 
- 说说你对语义化的理解？（美丽说） 
- 谈谈对web开发语义化的理解（搜狐） 
> 1.含义 
> 2.好处 
> 3.工作中的使用

####2.HTML中块状标签和行内标签的特点？（腾讯） 
- 哪些元素默认是块元素？（百度） 
- 行内元素和块状元素分别有什么？区别是什么？（乐视） 
- 块级元素，行内元素，行内块级元素有哪些？（美丽说） 
- 行内元素有哪些，块级元素有哪些？（猛哥科技） 
- img是行内元素还是块及元素？为什么 （大厨网） 
- 内联元素与块状元素有哪些，是怎么显示的？(大厨网) 
- IFC ? BFC ?

答案： 
- 块级元素(BFC => block formatting context 块级盒子的渲染模式):display:block 
> 1)独占一行,不允许其他的元素排在它后面; 

> 2)从上往下依次排列; 

> 3)块级元素的宽度是它父级元素的宽度，高度是它本身内容的高度 
> 4)块级元素可以设置盒子模型的所有属性- (width/height/padding/border/margin) 

> 5)ul/ol 后面紧跟着的只能是li;dl 后面紧跟着的只能是dt dd 

> 6)p标签不能嵌套任何的块级元素 包括它自己本身,也就是说p标签里面不能嵌套p标签

br,body,table,div,dl dt dd,ul li,ol li,footer,form,h1~h6,header,hr,p

####行内元素(IFC => inline formatting context 行内盒子的渲染模式)：display:inline 
> 1)不独占一行; 
> 2)从左往右依次排列,超过父元素的最大宽度会自动折行； 
> 3)宽高默认是它本身内容的宽高；要设置宽高需要转化块或者行内块元素display:block/display:inline-block;设置margin/padding 上下方向浏览器可以识别但是不起作用,只有左右起作用； 
> 4)行内元素里面不能嵌套块级元素,会提示报错; 
> 5)行内元素会因为空格键和回车键,影响元素之间的间距； 
> 6)对齐的方式是基线对齐； 
a,b,em,i,strong,span,sub,sup

- 行内块元素:display:inline-block; 
 - img input button select 
 - 可以设置宽高 还可以允许其他的元素排在它后面;既有行内元素的特点又有块级元素的特点 
> 1)从左往右依次排列,超过父元素的最大宽度会自动折行； 
> 2)可以设置盒子模型的所有属性; 
> 3)不设置宽高的时候,它宽高是它内容的宽高; 
> 4)行内元素会因为空格键和回车键,影响元素之间的间距； 
> 5)对齐的方式是基线对齐；

---------------------

###背景类（百度8个）
> 1.背景颜色 
background-color：#000 ； 
background:#000; 
例如：黑色（3种写法） 
black #000 rgb（0，0，0）

> 2.背景图片 
background-image 
url(‘图片的路径’)

> 3.背景平铺方式 
默认 repeat x和y轴同时平铺 
inherit 继承 （继承父元素的平铺方式） 
no-repeat 不平铺 
repeat-x x轴平铺 
repeat-y y轴平铺

> 4.背景是否随着滚动条的滚动而滚动 
background-attachment 
scroll 随着滚动条而滚动 
fixed 背景固定

> 5.背景位置 background-position:x轴的坐标 y轴的坐标； 
top/bottom/left/right/length(长度px)/百分比 
雪碧图:都要取负值；