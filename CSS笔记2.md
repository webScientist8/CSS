##CSS笔记2
---
[TOC]

---
###【css遵循规则】
就近原则:后面的代码会覆盖前面的代码;
默认的重置样式放在样式表的最上面;
reset.min.css 重置样式表

####【span 行内元素】
> 1)设宽度和高度属性不起作用,要想起作用，需要把它转为块级元素 display:block
> 2)设置padding/margin的上下浏览器可以识别但是不起作用,左右起作用

####【雪碧图/精灵图】 sprites.png/sprites.jpg
多个小图片合并在一张大图上
icons.png  小图标的集合
*** 雪碧图 background-position  都取负值; 默认的参考坐标 是雪碧图的左上角的点;

####【背景类backgroud】
> 1)backgroud-color 背景颜色
> 2)background-image 背景图片
>  3)background-repeat 背景平铺的方式
  repeat x/y平铺(默认值)
  no-repeat 不平铺
  repeat-x 表示x轴平铺
  repeat-y 表示y轴平铺
> 4)background-position 背景的位置

####【基线对齐】
- vertical-align  常用在一个小图标和文字内容在一行对齐显示
(图片:插入图片 img 单独用一个标签包起来)

####【腾讯的写法】
- 用height和line-height 也可以实现图片和文字的对齐显示(图片:背景图片 background-image)

####【定位】
- 绝对定位(position:absloute)
- 元素会脱离文档流,它需要找一个相对的参照物(position:relative),一般情况参照物是直接父元素,如果直接父元素也没有- - - -position:relative,它会继续往上查找,只到找到最外层的根元素html为止;
- 定位元素可以通过z-index改变层级,值越大,层级越高,越在上面;

-------------------------------------------------------------

- webstorm重命名快捷键:
shift+F6

###title标签里的内容是我们页面显示在浏览器页卡的部分;

####【定位】
绝对定位:position:absolute;
> 1)绝对定位元素会脱离文档流(元素漂浮起来了),而且它的位置被其他的元素占领;

> 2)通过上下左右(top/bottom/left/right)四个方向指定元素的位置;

> 3)方位同时有上下(top/bottom),跟着top的值走;
  方位同时有左右(left/right),跟着left的值走;
  
> 4)绝对定位元素一定要有相对定位的参照物(加在直接父元素上position:relative),如果父元素没有相对参照物，它会一层一层往上查找,直到找到最外层的根元素(html)为止;
> 
> 5)通过z-index能改变它的层级关系;

####相对定位:position:relative;
> 1)相对定位不会脱离文档流,它原本的位置还在,不会其他的元素占领;
> 2)通过上下左右(top/bottom/left/right)四个方向指定元素的位置;
> 3)方位同时有上下(top/bottom),跟着top的值走;
  方位同时有左右(left/right),跟着left的值走;
> 4)相对定位的参照物:是它自己本身;
> 5)通过z-index能改变它的层级关系;

####固定定位:position:fixed
> 1)绝对定位元素会脱离文档流(元素漂浮起来了),而且它的位置被其他的元素占领;
> 2)会固定在位置上,并不会随着滚动条的滚动而滚动;
> 3)通过上下左右(top/bottom/left/right)四个方向指定元素的位置;
> 4)方位同时有上下(top/bottom),跟着top的值走;
  方位同时有左右(left/right),跟着left的值走;
> 5)固定参照物:浏览器的窗口
> 6)通过z-index能改变它的层级关系;

####定位元素(绝对定位,相对定位,固定定位)的相同点：
> 1)都可以通过top/bottom/left/right四个方向控制它的位置;
> 2)都可以通过z-index改变元素的层级关系;

####定位元素(绝对定位,相对定位,固定定位)的不同点:
> 1.是否脱离文档流;
> 2.参照物;

- nav 导航栏  nav-wrap
- header 里面有一个网站的logo

####【文字内容对齐的方式】
- text-align:center   居中对齐
- text-align:left     左对齐
- text-align:right    右对齐

####【元素居中】
- 块级水平居中:margin:0 auto;
- 文字内容水平居中:text-align:center;
- 文字内容垂直居中：height和line-height的值设一样的值;


-------------------------------

打开设计稿:直接把psd的设计稿拖到ps中松开即可;

###【快捷键】
> 1)ctrl+1  设计稿100%显示;

> 2)ctrl+0  设计稿进来的状态;

> 3)按住空格键 出现一个小手 边按住空格键 边拖动设计稿;

> 4)设计稿放大/缩小  alt+鼠标滚动   还可以  ctrl +/- 放大/缩小

> 5)设计稿破坏,回到设计稿原本的状态: 窗口 - 历史记录

> 6)移动工具 - 在英文输入法状态下 V  自动选择移动要勾上(图层)

> 7)按住ctrl 点击图层空白的区域 会出现一个虚线框  在窗口下有一个信息(F8)面板可以看到虚线框的大小  logo 176*52
 在虚线框的基础上 ctrl+C(复制) ctrl+N(新建图层)  ctrl+V(粘贴)
 ctrl+shift+alt+S 同时按住 表示图片另存为  jpg png8 png24(背景透明)
 
> 8)如果图层有设计效果 -> 点到图层上鼠标右键 ->栅格化图层样式 ->变成一个纯图层
然后根据上面的操作 ctrl+C ctrl+N ctrl+v  ctrl+shift+alt+S 可以把图层保存下来

> 9)ctrl+N 新建图层  sprites 雪碧图/精灵图

> 10)填充前景色 alt+delete
   填充背景色 ctrl+delete
   
> 11)标尺 ctrl+R 从标尺上可以拉出参考线

> 12)按住shift键同时选中多个图层  ctrl+E 合并图层
 
> 13)取消虚线框的选区  ctrl+D

> 14)英文状态输入下 T  文字
 
> 15)取消被选中的状态 ctrl+enter

> 16)选区 M (英文状态输入法下)

> 17)选区的虚线框查看元素的大小尺寸 ->窗口 ->信息

- href="javascript:;   禁止a标签的默认链接跳转的行为

---------------------------------

###【css遵循规则】
- 就近原则:后面的代码会覆盖前面的代码;
- 默认的重置样式放在样式表的最上面;
- reset.min.css 重置样式表

####【span 行内元素】
> 1)设宽度和高度属性不起作用,要想起作用，需要把它转为块级元素 display:block
> 2)设置padding/margin的上下浏览器可以识别但是不起作用,左右起作用

####【雪碧图/精灵图】 sprites.png/sprites.jpg
- 多个小图片合并在一张大图上
- icons.png  小图标的集合
- *** 雪碧图 background-position  都取负值; 默认的参考坐标 是雪碧图的左上角的点;

####【背景类backgroud】
> 1)backgroud-color 背景颜色
> 2)background-image 背景图片
> 3)background-repeat 背景平铺的方式
  - repeat x/y平铺(默认值)
  - no-repeat 不平铺
  - repeat-x 表示x轴平铺
  - repeat-y 表示y轴平铺

> 4)background-position 背景的位置

####【基线对齐】
- vertical-align  常用在一个小图标和文字内容在一行对齐显示
- (图片:插入图片 img 单独用一个标签包起来)

####【腾讯的写法】
- 用height和line-height 也可以实现图片和文字的对齐显示(图片:背- 景图片 background-image)

####【定位】
- 绝对定位(position:absloute)
- 元素会脱离文档流,它需要找一个相对的参照物(position:relative),一般情况参照物是直接父元素,如果直接父元素也没有position:relative,它会继续往上查找,只到找到最外层的根元素html为止;
- 定位元素可以通过z-index改变层级,值越大,层级越高,越在上面;

【display】
- display:none;  让元素隐藏起来
- display:block; 让元素显示






