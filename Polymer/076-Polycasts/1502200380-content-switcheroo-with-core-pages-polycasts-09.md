
## Content Switcheroo with Core-Pages -- Polycasts #09

![video_screenshot](images/6x2A9UgLqEw.jpg)

** 视频发布时间**
 
> 2015年2月9日

** 视频介绍**

> Presto Change-O! Update the sections in your single page app using core-pages.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| Galory | 任皓 | —— | [ Youtube ]( https://www.youtube.com/watch?v=6x2A9UgLqEw )  |  [ Youtube ]( https://www.youtube.com/watch?v=W13blgxwfKo&index=39&list=PLvivLNHqjooz0jg-8ShYbWz4BERNNNR6Q ) | 1502200380 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

嗨  大家好

过得还好吧  

我是Rob Dodson罗布  多德森

在今天的Polycasts节目里  

我将向你们展示在使用core-pages元素的应用程序中

如何实现动态地切换

所有内容  那么开始吧

所有单页应用程序的特点是

当用户浏览不同部分时

它不会刷新整个页面

以Polymer网站为例

你可以看到  当我点击菜单条目时  

页面上的所有内容

都是几乎瞬间改变的

这使得整个应用有非常漂亮和轻快的感觉

有很多方法可以实现这个效果

最基本的  也就是我今天要讲的一个

包括显示和隐藏在页面上可用的

的不同的内容

简单说来就是把一些部分设置为display:block正常显示

而其他的部分设置为display:none不显示

还有些其他的办法

包括使用Ajax技术去和你的服务器对话 抓取一些内容

然后注入到文档中或是输送数据到

页面上已经存在的模板中

然后填充他们

好

我将在未来的课程里讲

其他的两个技术  但今天就从一个

简单的例子开始

就是让一些部分在显示和不显示间来回切换

这里我使用Sublime编辑器 而且已经准备好

建立了一个很简单的工程

在bower.json文件里  我已经包括了core元素

而且把所有内容安装到Bower Components目录里

那么继续进行  我将做的第一件事情就是

打开elements.html文件且把core-pages元素

加进去  它就被导入了

然后  在index.html文件的索引里  我将写出core-pages标签

同时把它的selected属性设为0

我还要进入并且设置些样本

内容

现在  这里的selected属性就很重要了

而且它工作的方式基本上是这样

告诉core-pages标签选择哪一个子元素去显示

这有点类似于数组里的索引

因此这个子元素将会是子元素0

这个子元素会成为子标签1  而这部分会是子元素2

因为我已经设置selected等于1

它将实际上使用了

下面这个portfolio节

如果你到Chrome上刷新页面

你应该看到那个portfolio content刚好显示在这里

但你不局限于使用数字索引

如果你给core-pages元素一个

带值的属性  你可以

选择匹配这个值属性的任何子元素

我要去设定值属性为data-category

这是一个我已经完全做好的属性

而且我将给每一部分

一个相应的data-category属性

现在  如果我设置选择的值为contact  这样就

让core-pages元素使用data-category属性是contact作为匹配值来

寻找子元素

看看我们的各个部分  我们可以

发现这个刚好匹配

因此  当我们跳转到Chrome更新这个页面时

我们会看到我们的Contact部分现在显示出来了

OK  如果你回顾一下上节课

我把所有的元素都放入一个自动绑定的template

元素里

现在  我们可以做同样的事

来把我们的core页面元素关联到一个菜单

让我们看一下

好的  我已经加了一些标记到我们的页面中

因此  我们有一个core-drawer-panel元素

它包含了我们所有的页面

我们也有core-header-panel和core-toolbar元素  一堆在之前课程里

讲过的元素

如果你错过了那些剧集

我们下边的显示注释里有相关链接

我要做的第一件事就是把所有一切包装

到自动绑定template之内

因此我将使用等于auto-binding的is属性

抓取我们所有的内容粘贴在里边

并且也要给我的template元素一个ID属性为app

那样的话之后我可以用Javascript引用它

下一步  我会弹开我的elements.html文件并

导入一个core-menu.html和一个core-item.html进去

回到我的index.html文件  我将写一个core-menu

并用和我们页类别相对应的core-item

来填充它

现在是魔法时刻

因为core-menu元素和core-pages元素扩展相同的公共父

叫做core-selector  这意味着它们

都可以利用到值属性的特性

我将给这里的每个core-item

一个data-category属性  它们匹配core-page元素的data-category

并且我将设定selected属性值等于一个局部

变量  我正在构造并命名为page

接着  我到core-pages部分

将selected属性赋值为一个局部变量

也叫做page

现在  事实上  我已经把这两个元素连接到起来了

我的菜单到我的页面

如果我打开Chrome并刷新页面

你将看到我在点击菜单项时

它同时也在更新页面的内容

为了设置一个默认页面  我要

在app.js文件里的选择自动绑定template元素

并给它的page变量一个初始值

我将更进一步并设置page变量等于home

现在  当我建立应用程序时

它会默认显示home网页

好  使用core-pages

在你应用程序中  你可以在不同状态之间改变

你可以开始考虑

添加像路由这样的额外的东西

那也是我们下节课要讲的内容

所以一定要订阅

一定要在下面留下评论

让我们知道您的想法

与往常一样  非常感谢您的收看，

下次再见




