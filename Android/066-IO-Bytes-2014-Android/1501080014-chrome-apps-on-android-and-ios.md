
## Chrome Apps on Android and iOS

![video_screenshot](images/vi/nU4lvgTrjFI.jpg)

** 视频发布时间**
 
> 2014年6月26日

** 视频介绍**

> Chrome Apps can now run on both Android and iOS using a toolchain based on Apache Cordova. This provides developers a strong incentive to adopt web technology to build native-like apps targeting desktop as well as mobile platforms. We'll be talking about the ease of development and the differentiating capabilities provided by the platform.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 周亿 | 程路 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=nU4lvgTrjFI )  |  [ Youtube ]( https://www.youtube.com/watch?v=nU4lvgTrjFI ) | 1501080014 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

嗨  大家好

我的名字是Max

我是Chrome团队的一名工程师

今天我将带领你用我最喜欢的方式去

通过Web技术来建立

非常棒的iOS和Android应用

你可以在你的移动设备上安装Chrome应用

首先  来介绍一下背景

你们当中的许多人可能已经知道了你们

为Android和iOS所创建的应用Web视图的

组件已经处于超负荷状态  如果你的应用程序

几乎完全是用HTML, Javascript,

CSS搭建的

现在要说清楚  这些应用仍然是

从App Store安装的

在主屏幕上有这个应用的图标

像其他的应用一样和对设备功能的

完整的访问权限

但是它们是使用Web技术建立的应用

我们通常把这类应用程序叫做混合应用程序

因为它们融合了Web应用技术和本地应用技术

在Android上  混合应用程序的一个缺点就是

Web视图在老版本的Android上

是有限制的

Chrome看到了这个问题并在Android上

做出了大量的改进  特别是在去年

但是运行在旧的Web视图上意味着

你不能使用这些改进过的优点

这就是为什么要引入

Intel Crosswork的开源项目

Crosswork项目提供了

一个嵌入式的双Chromium Web

在Android上的视图的版本就像

Ice Cream Sandwich一样

使用Crosswalk  混合的应用程序

可以运行在Chromium的最新版本上

而不需要关心Android系统的版本

在iOS上也是相同的  Web视图自从iOS6

以来已经有了很大的升级

现在  有了iOS8  Web视图

将会拥有Safari浏览器的全部功能

说了这些是什么意思

它意味着当我们去建立一个混合型的应用

使用了现代的Web视图可以运行在几乎

过去三年内所有发布的

Android和iOS设备上

这里是一个基于HTML5 Canvas元素的

在Crosswalk的Web视图上的

叫做Pop Pop Win running的游戏

Canvas元素的硬件加速使得画面没有任何的锯齿

在几年以前这是根本不可能的

现今  混合型的应用程序可以使用例如

WebGL, WebRTC, Web Audio的

技术加速2D的Canvas元素

例如像现代的Web工具包Polymer

最佳的性能状态不需要

浏览器对polyfills的支持

甚至它做的更好

混合应用程序是不限制于只使用Web API的

因为这些应用是本地应用

你会有完整的访问到

Android和iOS设备API的权限

例如身份验证  云端信息  通知

付款  蓝牙  套接字  摄像头  和更多的内容

这款应用使用了Polymer技术显示出了

一些非常好的动画效果

完全不需要运行polyfill

所以很显然很多人都喜欢去开发混合型应用程序

但是你如何开始进行应用开发

我们的团队花了一年的时间开始

对流行的开源的混合应用程序进行资源整合

Apache Cordova工具包

我们同样看到了为Chrome桌面应用

打包的伟大的工作已经完成了

所以  在一月份的时候  我们发布了预览版的

开发者工具CCA  可以使用已经打包过的

Chrome应用格式去建立混合的移动应用

现在Web开发最方便的一点是

非常快速的工作流程和非常短的反馈回路

不需要编译  你可以直接改变某些内容

然后立刻就可以看到效果

但是混合型的应用程序就像本地的应用一样

你必须要等待编译完成

所以你就失去了非常快的反馈回路

我们的配套工具  Chrome移动应用开发者工具包

改变了这一切

让我来为你展示它是怎么工作的

我通过USB连接了我的设备

但你也可以使用Wi-Fi来连接

我在设备上运行了App开发者工具

现在我输入一条命令将我的应用推送到设备上

并等待变化

你可以看到这个app被传输到了设备上

并且随着App开发者工具包一起运行

现在在右上角的那个设置按钮

有一些小  现在让我们来把它变得大一些

现在打开CSS文件

一旦我打开了  我们会把它以2的倍数来放大

一旦完成  我将保存这个文件

文件的修改被检测到并推送到设备

并且App重新运行了

设置按钮变得更大  看起来比刚才好多了

我们将设计我们自己的并且更大的一个图标

现在让我们进入那个设置菜单

OK  它没有响应

让我们来看看吧

我知道处理点击操作的控制器

在weather.Js文件中

我将打开那个文件

是的  那些内容被我注释的太早了

去掉那些注释然后保存这个文件

再一次的  刚才做过的修改被检测到了

希望它能一次加载成功

是的  设置按钮现在可以用了

无需重新编译

我会继续慢慢的并即时的调整

我手机上的应用程序

同时我们也在努力支持同样的编辑的工作流程

在Google开发编辑器上进行更新

你可以在Google I/O

进行在线交谈和学习

你会在这里拥有这一切

Chrome应用程序的伟大之处在于它支持多平台

包括Windows, Linux, Mac,

Chrome OS, Android和iOS

在移动设备上使用Chrome应用程序

你可以使用所有的最新的和最伟大的混合应用程序的技术

然而  这比以往任何时候都容易的多

我们很期待能见到你所创建的应用程序