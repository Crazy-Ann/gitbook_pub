## App Indexing API 

![video_screenshot](images/UjLJoMWSXts.jpg) 

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> In this session we'll give an overview of the new App Indexing API for Android that lets you specify links -- through your app itself -- for App Indexing. It also gives you a way to re-engage users through Google Search App autocompletions. We'll provide step-by-step guidelines for how to get started. 

** 视频推介语 **

>  暂无，待补充。

### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| 兰州夏菜二厂  | 韩淼 | 暂无 | [ Youtube ]( https://www.youtube.com/watch?v=UjLJoMWSXts ) | [ Youtube ](https://www.youtube.com/watch?v=pwxXMfTQ1QY) | 1504020507 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator ) |


### 解说词中文版：

嗨  我是Lawrence Chang  谷歌的应用目录的

高级产品管理师

在本节中  我将给你一个APP索引目录的全览

并告诉你如何使用它

现在应用目录索引代表了谷歌搜索的一种能力

它可以帮助用户查找和访问本地应用就像在网站上那样

对于APP开发人员

APP目录给你提供一个驱动APP的机会

通过谷歌

APP目录API将这个机会拓展了

首先  APP目录提供给你一个方法

来指定映射地图通过网站的标记和链接地图

APP目录API提供了第三种选择

你可以使用它指定应用程序的链接

在这种情况下  通过应用程序本身

第二  当APP目录添加APP的硬链接给搜索结果

APP索引目录API添加了APP的硬链接

使查询自主完成

自动完成个性化提供给用户

基于用户APP的内容

与之前预期的一样  所以可以帮助用户重新进入应用程序

当开始使用APP索引API

首先你的APP要支持深链接

你可以跟随我们的指导去了解如何做到这一点

然后我们也建议你跟随我们的通用APP索引

与你所需要的一样

这包括将你的网页链接到APP

你可以在我们的开发者指导中了解更多

当你完成了这些步骤后

然后开始考虑APP索引API

所以让我们来看看更多细节

首先  你需要将Google Play服务添加到你的APP中

如果你还没有

为完成这个  添加一行代码到你的清单文件中

去得到一个正确版本的Google Play服务

然后  如果你使用Android Studio

你还需要添加一个依赖你的构建文件

最后  获得最新版本的谷歌服务

通过SDK管理器

然后在主要文件中带入应用程序索引

和应用程序索引链接类文件

接下来  你定义一个全球谷歌API用户

然后在onCreate中将它实例化

在onStart里联系你的客户

并同时定义你的APP地址和响应网页地址


现在在这个例子中我将向你展示字符串的真正的链接

但是在显示中  你会通过编程方式实现

定义这些链接的变量和参数

然后定义定义这些链接在页面上

包括APP和web地址

一旦你定义出站链接

你创建应用程序索引链接对象

同归提供应用程序地址  网址和视图ID

然后  你创建一个列出这些内容的链接

接下来  定义当前页面的标题

这个标题是自动完成用户所看到的UI

现在  你已经准备好调用API应用程序索引视图方法

你作为参数提供Google API客户端

活动  和应用链接标题  网页链接和列表

和你刚刚创建的出站链接

最后  在onStop中添加一个调用viewEnd的方法

来断开你的客户

所以最为总结  如果你想得到大部分的

应用索引  你应该开始添加硬链接

来支持你的APP  然后跟随我们的通用APP目录指导方针

最后  实现APP索引API

有关更多信息  可以参见我们的开发者指南

我是Lawrence Chang

感谢观看