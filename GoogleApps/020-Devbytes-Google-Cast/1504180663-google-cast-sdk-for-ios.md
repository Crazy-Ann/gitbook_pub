
## DevBytes: Google Cast SDK for iOS

![video_screenshot](images/9jkwjAPas_8.jpg)

** 视频发布时间**
 
> 2014年2月5日

** 视频介绍**

> Learn how to cast content from iOS apps to Google Cast receiver devices such as Chromecast. This video gives an introduction on how to build Google Cast sender applications for iOS using the Google Cast SDK

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 艾雪媛 | Wallace4ever | —— | [ Youtube ]( https://www.youtube.com/watch?v=9jkwjAPas_8&index=2&list=PLOU2XLYxmsILfBNIVzWsfIscQCxso4gfs )  |  [ Youtube ]( https://www.youtube.com/watch?v=Hw3Upx6N4qA&index=17&list=PLvivLNHqjoowcHLv6e2X2TpT08IDKOV1H ) | 1504180663 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

大家好 我的名字是Kevin Nilson

我是Google Cast的开发者

我来给大家简要地介绍一下iOS版的Google Cast SDK（Google投射软件开发套件）

Google Cast SDK可以让你将iOS以及

Android和Chrome应用中的内容 

通过像Chromecast这样的Google Cast接收器投射到第二个屏幕

Google Cast可以让你使用你所熟悉的控制器

如手机 平板 或者浏览器

来在大屏幕中控制使用你的应用程序

我们先看一下iOS版的Google Cast发送应用程序的

生命周期

首先  你必须在你的网络中搜索设备

一旦找到设备  用户就可以

选择一个设备与设备管理器进行连接

连接之后 你将能启动你的应用程序

而最终在应用程序启动之后

你可以开始发送和接收消息了

现在  我们看看Cast图标

只有在你从网络中找到设备之后

你才能把Cast图标显示出来

如你所见  在这个例子中 当用户点击

Cast图标之后 你应把可连接的Cast设备列表

显示出来

而为了显示设备列表

你需要先开启deviceScanner进行扫描

在扫描了几秒之后

你就可以从Device Scanner中得到网络上的设备列表

每个设备对象都有一些属性

例如  可以向用户显示友好的名称

在扫描时  对每个找到的设备

DeviceDidComeOnline代理会被调用

记住  你不需要手动去

记录这些设备  因为DeviceScanner已经

保存了一份设备列表

但是 你也可以使用DeviceDidComeOnline回调函数来

触发刷新设备列表的操作

并将刷新信息显示给用户

Cast图标有两个主要的状态  断开和连接

当一个投射设备被连接上之后

你必须要改变Cast图标的颜色为突出显示的颜色

连接状态的图标颜色可以自己定义

以便跟你的应用程序的主题颜色相匹配

你可以看到  在这个Cast视频样例程序中

我们采用黄色作为连接状态

同时 还有个中间状态

用来表示Cast接收器正在连接

这是为了在Wifi网络的连接速度缓慢的时候使用的

这个状态下  Google Cast按钮会显示动画

在左下角的Google Cast按钮中的波纹

会逐渐变成连接状态的颜色

为了连接一个设备

你要为选中的设备初始化一个DeviceManager

然后你可以连接该DeviceManager

当DeviceManager连接之后

它会调用DeviceManagerDidConnect代理方法

现在在设备连接之后  你可以使用从开发者门户收到的

应用程序序列号来启动你的应用程序

启动应用程序时会使HTML5接收程序启动

从而给你带来10英尺的体验

一旦你的程序启动

你就可以发送和接收消息了

你必须为投射信道分类  从而向你的

Google Cast接收器发送和接收文字消息

多媒体控制信道是一个投射信道的子类

它是非常适合用在控制多媒体方面的子类

现在 你应该对Google Cast应用程序

的生命周期有一个很清晰的认识了

当你打算把Google Cast

加入到你的应用程序时 我建议你们读一下设计清单

遵守这个清单 你的应用程序

就会兼容普通的用户接口模式

这种模式用于所有的Google Cast发送应用程序中

保证你的程序 简单 直观 可预测

每个Cast应用都采用相同的模式

会使所有的用户受益

遵循这些指导 可以使你的用户在使用Google Cast时

避免遇到麻烦

为了帮助你实现最好的应用实践

我们提供了一系列项目的清单

包含完整的描述和图片

你可以再developers.google.com/cast中得到

更多的关于Google Cast SDK的信息

不要忘记看一下Cast设计清单

你可以在github.com/googlecast中得到一些例程

如果有问题 就在Stack Overflow上提问

标记为#google-cast

你也可以在Google+上 加入Google Cast开发者团体

在那里你可以得到一些技巧 分享你的经验

现在你就可以开始写你的iOS Google Cast

发送程序了

享受乐趣吧




