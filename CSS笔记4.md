##CSS笔记4
---
[TOC]

---

- 编辑器:webstrom  atom  sublime
- 浏览器:谷歌 -webkit

###【PC和移动端区别】
- PC处理浏览器的兼容问题
- 移动端 处理手机的适配 -webkit

####PC鼠标移上  点击切换
- 移动端 没有鼠标  手指(单指/多指) 滑屏

####【vieport 视口】可视区域的大小
- meta:vp  tab
- 注意：移动端的H5页面必须要加上视口的代码
- width=device-width宽度等于设备的宽度
- user-scalable=no 是否允许用户手动缩放页面
                 no 禁止/yes 允许
- initial-scale=1.0  初始的缩放比:1.0
- maximum-scale=1.0  最大放大比1.0
- minimum-scale=1.0  最小缩放比1.0

####【video视频播放器】
- src="视频播放器的路径"
- autoplay="autoplay" 自动播放
- loop="loop"  循环播放
- controls="controls"  控制条

####【产品的类型】
> 1.PC和移动端 公用一套页面结构 html(简单结构)
  媒体查询(猎豹浏览器  华为)
> 2.PC和移动端分开(京东 淘宝 网易 新浪 凤凰)
> 3.自适应(百分比) 自然堂


--------------------------
###背景类（8个 : 百度面试题）

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

> 6.背景的大小尺寸 background-size 
cover 覆盖 拉伸 
contain 留白

>7.背景定位的区域（显示的起点）background-origin 
border-box 从边框的外边（包括边框）开始显示图片 
padding-box 从内边距（包括内边距）开始显示图片 
conntent-box 从内容区域显示图片

> 8.指定背景图像的绘画区域(保留) 
border-box 保留边框的部分 
padding-box 保留内边距部分 
content-box 保留内容部分
【box-sizing 怪异盒模型】 
border-box 会把padding和border的值都算在宽度里面 （怪异盒模型） 
content-box 不会把padding和border的值都算在宽度里面 （正常盒模型）

####【animation css3动画】 
> 1.通过@keyframes 动画的名称 - 关键帧写好动画； 
> 2.元素去调用动画名称 ；

####【animation 8个】 
> 1.animation-name 动画的名称 

> 2.animation-duration 动画持续的时间 
持续时间越长 动画越慢 
反之 动画越快 

> 3.animation-timing-function 动画运动曲线 

> 4.animation-delay 动画延迟的时间 

> 5.animation-iteration-count 动画运行的次数（1 infinite无限次） 

> 6.animation-direction 动画运动的方向 

> 7.animation-play-state 动画运动的状态 

> 8.animation-fill-mode 动画结束保持的状态

------------------------------------

###动画

- 设计稿 750*1334(iphone6) 
- 设备的分辨率 375*667 
- DPR：2.0（device pixel ratio）设备的像素比

####【封页动画】 
> 1.bounceInDown 
> 2.bounceInLeft 
> 3.bounceInRight 
> 4.fadeInLeft 
> 5.bouceInUp

> ps反选：ctrl+shift+i

####【媒体查询】 
- pc和移动端公用一套页面结构 
> 1.@media 媒介 
- 2.媒介的类型 
 - all 所有的类型 
 - screen 移动设备（手机） 
 - print 打印机 
 - TV 电视 
-  3.连接符 
 - and 和 
 - only 仅仅 
 - not 排除 
- 4.（条件） 
- 5.{ 
css代码快 
}

####【rem】font size of root element 
- 根元素的字体大小（html）
