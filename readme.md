#ife 2017
##Demo

task1.1 在线预览地址：http://htmlpreview.github.com/?https://github.com/lawlietfeng/ife2017/blob/master/task1.1/.idea/task1.1.html

task1.2 在线预览地址：http://htmlpreview.github.com/?https://github.com/lawlietfeng/ife2017/blob/master/task1.2/task1.2.html

task1.3 在线预览地址：http://htmlpreview.github.io/?https://github.com/lawlietfeng/ife2017/blob/master/task1.3/task1.3.html

task1.4 在线预览地址：http://htmlpreview.github.io/?https://github.com/lawlietfeng/ife2017/blob/master/task1.4/task1.4-flax.html

task1.5 在线预览地址：http://htmlpreview.github.io/?https://github.com/lawlietfeng/ife2017/blob/master/task1.5/task1.5.html

task1.6 在线预览地址：http://htmlpreview.github.io/?https://github.com/lawlietfeng/ife2017/blob/master/task1.6/task1.6.html
###**notes**
###**task1.1 面向零基础的HTML代码编写**

 - `ol`有序列表，`ul`无序列表
 - `img`的`alt`属性最好写上简介，有利于seo，判断图片与文字是否相关的依据
 - `colspan="2"`属性规定单元格可横跨的列数，这里为2列
 - H5属性`placeholder`属性提供可描述输入字段预期值的提示信息（hint）。该提示会在输入字段为空时显示，并会在字段获得焦点时消失。
#### **对于html语义化的理解** 
根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的!同时让浏览器的爬虫和机器很好地解析。
为了在没有css的情况下页面也能呈现出比较好的内容。
对于用户体验更好，例如`title`、`alt`用于解释名词或解释图片信息、`label`标签的活用。
有利于**SEO**，让网页和搜索引擎建立良好沟通，有助于爬虫抓取更多的有效信息，爬虫依赖于标签来确定上下文和各个关键字的权重。
方便其他设备的解析（如屏幕阅读器、盲人阅读器、移动设备）以意义的方式来渲染网页。
便于团队**开发和维护**，语义化更具可读性，是下一步吧网页的重要动向，遵循W3C标准的团队都遵循这个标准，可以减少差异化。

                         <heraer>
                         <nav>
        <article>                               <aside>
        <section>
                         <footer>
如上结构没有用到一个`div`的分割，都是用html5的语义标签。却也不能因为这些新标签的出现，随意用之。所以有些地方还是要用`div`的，就是因为`div`没有任何意义的元素，他只是一个标签，仅仅是用来构建外观和结构。因此是最适合做容器的标签。


###**task1.2 零基础HTML及CSS编码（一）**

 - css3：`box-shadow` 向框添加一个或多个阴影  例：`box-shadow: 2px 2px 2px black;`
   x轴右移2px，y轴下移2px，模糊距离2px，黑色
 - `font-weight: normal;`去掉加粗效果
 - 字体unicode编码网址：http://code.ciaoca.com/style/cssfont2unicode/
 
 在 CSS 中设置字体名称，直接写中文是可以的。但是在文件编码（GB2312、UTF-8 等）不匹配时会产生乱码的错误。为此，在 CSS 直接使用 Unicode 编码来写字体名称可以避免这些错误。使用 Unicode 写中文字体名称，浏览器是可以正确的解析的。
 
 - 无序列表`ul>li`最左的圆点可以用`list-style-type:none`来去掉。
 
 - 表单要被form所包裹，不能漏啦！！
 
###**task1.3 三栏式布局**

 - `overflow`  ：属性规定当内容溢出元素框时发生的事情
 
**visible**	默认值。内容不会被修剪，会呈现在元素框之外。

**hidden**	内容会被修剪，并且其余内容是不可见的。

**scroll**	内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。

**auto**	如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。

**inherit**	规定应该从父元素继承 overflow 属性的值。

这里使用`overflow: auto;`来包裹子元素，让父元素跟随子元素的变化而变化

 - `position`属性
 
**inhert** 从父元素继承position属性值

**static** 默认值

**relative** 相对定位，相对于元素本身定位，例如：`left:20px;`此时是针对元素自身左移20px。

**absolute** 绝对定位，相对于 **static** 定位以外的第一个祖先元素进行定位。元素的位置通过 **"left", "top", "right" 以及 "bottom"** 属性进行规定。

**fixed** 相对于浏览器窗口的绝对定位，例如屠龙宝刀点击就送类型的跟随窗口的广告就是这样定位的。

 - `float`浮动的各种应用场景：http://www.cnblogs.com/dolphinX/archive/2012/10/13/2722501.html

###**task1.4 定位和居中问题**

水平垂直居中的几种办法

 - **负外边距(Negative Margins)**

  `position: absolute;
  
   top:50%;
    
   left: 50%;
    
   margin-left: -（width+padding）/2;
    
   margin-top: -（height+padding）/2 ;`
    
优点：

.良好的跨浏览器特性，兼容IE6-IE7。

.代码量少。

缺点：

.不能自适应。不支持百分比尺寸和min-/max-属性设置。

.内容可能溢出容器。

.边距大小与padding,和是否定义box-sizing: border-box有关，计算需要根据不同情况。

 - **Flexbox**

 `display: flex;
 
 justify-content: 
 
 center;align-items: center;`

优点：

.内容块的宽高任意，优雅的溢出。

.可用于更复杂高级的布局技术中。

缺点：

.IE8/IE9不支持。

.Body需要特定的容器和CSS样式。

.运行于现代浏览器上的代码需要浏览器厂商前缀。

.表现上可能会有一些问题

其他居中的办法：http://blog.csdn.net/freshlover/article/details/11579669
    
###**task1.4 零基础HTML及CSS编码（二）**

 - 用一个div层包裹左边的元素，然后让右边的元素向右浮动，再加上overflow的效果来包裹住因为页面放大缩小之后而变化位置的图片栏就完成了。
 - 可以参考这个网站[老生长谈：css实现右侧固定宽度，左侧宽度自适应][1]说的。
 - 本来想试试那个`display:table`和`display:table-cell`的，好用是好用。但是不熟，发现有的div设置了margin什么的都会无效，所以没继续用了。
 - 暂时不考虑兼容问题，ie9以上是没有问题的。

###**task1.4 通过HTML及CSS模拟报纸排版**

 - `opacity`:设置透明度1~0逐渐消失
 - [用css制作三角形][2]


  [1]: http://jo2.org/css-auto-adapt-width/
  [2]: http://www.jb51.net/article/42513.htm
