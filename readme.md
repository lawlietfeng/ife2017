#ife 2017
##Demo
task1.1 任务要求地址：https://github.com/lawlietfeng/ife2017/tree/master/task1.1

task1.1 在线预览地址：http://htmlpreview.github.com/?https://github.com/lawlietfeng/ife2017/blob/master/task1.1/.idea/task1.1.html

task1.2 任务要求地址：https://github.com/lawlietfeng/ife2017/tree/master/task1.2

task1.2 在线预览地址：http://htmlpreview.github.com/?https://github.com/lawlietfeng/ife2017/blob/master/task1.2/task1.2.html
###**notes**
###**task1.1 面向零基础的HTML代码编写**

 - `ol`有序列表，`ul`无序列表
 - `img`的`alt`属性最好写上简介，有利于seo，判断图片与文字是否相关的依据
 - `colspan="2"`属性规定单元格可横跨的列数，这里为2列
 - H5属性`placeholder`属性提供可描述输入字段预期值的提示信息（hint）。该提示会在输入字段为空时显示，并会在字段获得焦点时消失。
#### **对于html语义化的理解** 
根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的![此处输入图片的描述][1]同时让浏览器的爬虫和机器很好地解析。
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
