
## Lightning Talk: Automate Publishing for Google Play APIs

![video_screenshot](images/rswSiFTENSM.jpg)

** 视频发布时间**
 
> 2015年3月12日

** 视频介绍**

> Watch the complete GDC '15 playlist at: http://goo.gl/whR0PLFind out just how much of your Android game publishing process you can automate with a tiny shell script using APIs from Google Play and Google Play game services.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 虞高 | wang7x | —— | [ Youtube ]( https://www.youtube.com/watch?v=rswSiFTENSM&index=13 )  |  [ Youtube ]( https://www.youtube.com/watch?v=ASWIhvS2wR0&list=PLvivLNHqjoowK2IZ9j_NYIucUrGgdiDrT&index=45 ) | 1504150639 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

嗨 我是Bruce

我是一个Google Play Game Service 小组的工程师

今天，我将向大家分享一些

我们刚完成的新的特性

来帮助你们自动化你们的游戏向Google Play的发布过程

带着我们全新的API

首先  先介绍一些我们小组

我们Google Play Game Service主要负责什么呢？

这是云服务的一个分支  例如成就系统

［没听清］  在线多玩家  云存储和读取

呃呃 我建议大家先了解一下

假如说你要创建一个游戏

你想要每天给你的内测用户发布内侧版本


那么你可能会想让你的游戏本地化  翻译成不同语言

或者你的设计师会抓狂

他有许许多多的成就想要加到游戏中

那么首先  你应该去Google Play Developer控制台看看

一个个把这些元数据加进去

我们收到了很多你们的建议

许多开发者有大把无聊的时间来做这些

所以我们加入了两个新的API来帮助你们

首先是Google Play Game Services 发布的API

第二是Google Play Developer Publishing API改

这两个可以帮你们分别

管理游戏服务和你的商店数据

开始用这些API 你的第一件事情就是

去开发者控制台  点击设置

获得这些API权限

从这里开始  你可以按照步骤设置API

你一旦做了这个  你就能得到这些API的权限

举个例子  这是我们的成就系统API

你可以获取  更新  删除  插入  以及排列他们

我们同时有一个API可以上传这些成就的图片

我们假设你的成就已经搭建好了

你想要获取这样的API给你的成就系统

这里有一个例子

你用你的成就ID创建一个HTTP请求

得到它的JSON响应

更新的话也是差不多的

同样的URL

这就是一个获得请求

而且你可以改变JSON数据并且更新

一个重要的提示你要先获取（get）

在你更新以前  因为

我们就是这么处理同时发生的更新的

这有个例子是关于Google Play developer API的

你必须要先创立一个我们称之为edit的东西  这本质是一个

可变的列表

你可以编辑这个edit

回到之间的例子

假设你每天要发布alpha测试

你要做的就是创建一个edit 更新你的APK

设定你APK的内测版本  最终创建那个edit

还有你可以在上面的过程中加很多其他步骤

这里有一个列表关于你可以做的事情

你可以改变你的截图

你可以改变你的Play 商店细节  管理你的测试人员

增加更多的本地化 

到现在你可能想知道

如果其他开发者想要获得你的数据怎么办

不用担心

我们权限管理十分严格

你可以在你的Developer Console中管理它

并且仅有游戏的拥有者才能获取这些数据

我们也有两个主要的方法来进行客户端认证

第一是OAuth 客户端通过这个OAuth代码

一个常见的错误是没有加上这个代码

记住要加上它们

第二种错误是使用服务账号

服务账号其实就是一个另外的账号

这个账号同样被准许了权限

这个是很常见的因为你能部署一个创建好的服务器

然后用这个服务账号来跑发布测试过程

不要忘了  Google Play Games同样是跨平台的

所以当你更新你的成就数据时

它在你的所有平台上都有效

你不用再这方面担心

有了这些  你应该能自动化你的

游戏发布过程了

并且希望  这能帮你节省时间

你能最终好好利用这个时间来

吃点蛋糕什么的


如果你还有疑问  可以看看Github上的例子

我们有Python 和JavaScript

还有我们有Java的例子关于Google Play Developer API Edits

十分感谢您的收看






