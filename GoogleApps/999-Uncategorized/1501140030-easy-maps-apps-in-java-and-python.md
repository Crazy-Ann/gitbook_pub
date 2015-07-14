
## Easy Maps Apps in Java and Python

![video_screenshot](images/2s7UAscFUDw.jpg)

** 视频发布时间**
 
> 2015年1月7日

** 视频介绍**

> Integrating Google Maps API services into applications provides a great set of location based services for powerful functionality. If you write server side applications in Java or Python, accessing these APIs requires some way to talk to the Google Maps server REST APIs that provide the interfaces.Google have built an open-source set of client libraries that take care of all the nitty-gritty detail of connecting, and managing Maps API services for both Java and Python.Alex Danilo introduces these libraries, and what they do - allowing Java and Python server side application developers to save time integrating Maps API services into their applications.These libraries streamline and simplify the work required to get an application up and running by taking care of things like retry for dropped connections, rate limiting to make sure applications manage their quota, and more.Documentation for the client libraries is on the Google Developers Site here, and the open source project code is on github here.If you develop in Java or Python, you should definitely take a look.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 姜昭宇 | 程路 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=2s7UAscFUDw )  |  [ Youtube ]( https://www.youtube.com/watch?v=eHY1CPur8VA ) | 1501140030 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

嗨

作为一个开发者  我知道我的时间是宝贵的

一寸光阴一寸金嘛

并且产品上市的时间更为重要

所以当我开始构建一个应用程序的时候

我第一件要做的事情就是去

找到一些类库来提升开发速度

我是Alex Danilo  我将向你介绍

Google地图API中的一些非常强大的类库

现在有了Google地图以及相关API

您可以建立一个功能非常丰富的应用程序

把基于地理位置的服务(LBS)模块

集成到您的应用程序中

但是  当你尝试这样做的时候很快就会令人望而生畏

我们为很多客户端做了类库

让你的工作更轻松

这些库原生支持

Java和Python语言开发的服务器端

因此  他们所做的是使用我们现有的API的接口

比如Directions API, the Distance Matrix API

the Elevation API, the Geocoding API和the Time Zone API

这些API接口让你的开发更简单

通常情况是这样的  当你在某些应用程序下

需要使用Google Maps时  则你需要实现

服务器端提供的RESTful架构

状态无关(stateless)的接口

当然  如果你更倾向于使用不同的语言去开发

例如Java或Python  那这工作量就大了

我们已经为你做好了不同客户端的类库帮助你

建立与这些服务之间的连接

并且提供相关语言的接口

所以你不必把Java接口转换为JavaScript接口

或者其他接口之间的互相关联等

现在有这种方法的以下几个优点

一是我们已经帮你做好并测试通过

你知道它是一定可行的

二是它减少了代码量

这个就是实际的编码量

你只需要处理实际的业务即可

现在这样做的美妙之处在于  已经建立的这非常棒的

客户端库的API  它会给你一个简单的接口来工作

不仅如此  它会处理认证和秘钥

如果有这样的模块  你的应用程序

的开发可能会有点复杂

但我最喜欢的功能之一就是重试(Retry)

重试所做的是  当服务器可能

出现了间歇性故障或者是极不稳定的网络连接

或者是类似的情况

特别是在移动网络

它会直接忽略

什么都不会发生

这简直棒极了

有很多人可能喜欢的另一件事是速率限制

所以它所做的是限制了到服务器的连接

这样你就不会碰上造成超出您的

配额限制的错误

这个类库可以按照你设定的速率查询

从而让应用程序避免

任何超出配额而导致的错误

也许最重要的事情是

在整合这些类库到你工程里的时候

你实际上是在处理本地对象

所以如果你正在使用Java

你会真正的去操控一个Java对象

所以调用方法直接操作Java对象

Python已经很简单了

为了节省时间就不需要处理

直接返回即可

所以你不必花时间去组建一个URL地址或

通过JSON传输将结果  这样可以节省你

手动设置模型映射的时间

另一个好处是  如果你使用Java的库

它可以让你进行同步或异步连接

要如何运行连接这便是你的选择了

最重要的是  这整个客户端库集是开源的

所以如果你喜欢可以修改它或做出你自己的贡献

要了解更多的信息  跳转到我们这个URL的文档

您也可以从这里  我们的Github资源库查看

Java和Python的源代码

我们很乐意看到你构建的应用程序

并且我们很想让你告之  想要让我们随后支持

哪些语言

我是来自Google开发者平台团队的Alex Danilo