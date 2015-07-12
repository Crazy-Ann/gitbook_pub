
## Game On! - Flatbuffers

![video_screenshot](images/iQTxMkSJ1dQ.jpg)

** 视频发布时间**
 
> 2014年月21日

** 视频介绍**

> Data serialization is vital to all modern games, but choosing the wrong format can cause bloated files that take longer to load. Flatbuffers are a data serialization library that focuses on creating the smallest serialized files with the fastest load time possible.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 陈林 | 黄莘 | ——| [ Youtube ]( https://www.youtube.com/watch?v=iQTxMkSJ1dQ )  |  [ Youtube ]( https://www.youtube.com/watch?v=iQTxMkSJ1dQ ) | 1505050794 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

你开发的手机游戏似乎已经表现的非常好

但是用户还会抱怨游戏加载时间

经过分析  问题变得很清晰

你花了太多时间用于数据序列化

我叫  Colt McAnlis  我们能提高用户数据加载

速度并且让你更容易使用

使用新的 flatbuffer 库

你肯定知道  加载内容是一个不流畅的过程

所有内容都来自内容创造工具

如物理设备  动画  电子表格数据

这些都必须以某种格式存储

以便加载到游戏中  传给用户

这甚至会统计临时文件

如通过网络发送游戏数据

或者保存到游戏以便以后加载

因为这对于游戏开发至关重要

因此我们该怎么优化它的性能呢

怎么做  让我们回到基本问题

序列化的过程就是把内存中的数据结构

转化成一种数据格式  这种格式

能被再次转化成内存中的数据结构

将来  信息存储更紧凑

以便节约存储空间

现在一些流行的序列化数据格式

XML和JSON  主要是因为用户可读

也可以通过文本编辑器打开

查看  修改  并且也知道

自己在怎么操作

这个流行性可以让它扩展到支持本地语言

如C# Java和JavaScript

但是事实上  这些格式有一些严重的缺陷

首先  它们过于庞大

实际上  文件格式可阅读

意味着有许多冗余的语法

让文件更容易阅读和使用

这就使文件大小比实际需求要大很多

其次  这些格式过于僵化

给反序列化带来了巨大的压力

解析系统必须读取string数据

然后分析数据

以确定转化成内存中的数据类型前的

实际数据类型

当你的格式支持高级类型的时候会变得很糟

如GUID  时间戳和数据对象

结果就是  反序列化过程变得很慢

一旦复杂性达到一定水平

为了解决这问题  我们为游戏开发出一个新的开源工具

叫做flatbuffers

这个库能让它自己回到基本的序列化状态

也就是说  能很快的编码和界面

并且生成最好小的编码文件

现在用一种高级方式

flatbuffers通过创建一个序列化数据类型描述文件

叫schema

通过一个语法编译器来操作

编译器产生一个代码文件  可以放到你的应用里

来编码或者解码你定义的数据格式

因为游戏里的structures比较复杂

放入编译器的schema格式

可以是描述数据格式的

原始relation 如可重用的类对象

枚举和非常基本的类型

这个布局允许flatbuffers是类型安全的

将来可以允许你读取序列化数据

而不需要进行类型转换

内存分配或者加载的时候解包数据

这将极大提高速度

只要你为所有的序列化数据

创建schema文件

你把这些schema文件放到平台的C编译器里面

就会为游戏产生源代码文件

使用正确的命令行switchs

也可以产生C++和Java

甚至是Go代码文件  你也可以顺便放进你的项目里面

和再次编译

现在  不管你使用什么语言编程

使用flatbuffer加载数据真的很简单

给你序列化的字节流

就可以转化成单行代码

转化成你想得到的对象

然后你就可以阅读使用了

现在这一切都是极好的吗  它到底有多快呢

让我们看看flatbuffer和其它

option的比较  协议buffer和JSON

我们可以看到对于编码和解码时间

flatbuffer比其它格式表现优秀

实际上  我们并排起了对比的话

我们看见在图里面flatbuffer耗得时间是极少的

嗯

同样  编码后测试数据的大小也是很重要的

你可以看到

flatbuffer编码和解码耗时时间非常短

当它变成原始数据大小的时候

同样的zlib压缩的时候

更多的是

你知道当你改变游戏数据格式的时候

会引起极大的混乱

相对于旧数据  还能动态构建  能兼容吗

Flatbuffer不存在这样的问题

它提供了可以改进schema的功能

不会影响旧数据和就工程的兼容性

我觉得它很棒

当然  它还有很多其它很好的功能

等待你去发现

想要了解更多flatbuffer库

或者想了解更多还没被发现的信息

请查看flatbuffer文档

然后在我们的github里面下载代码来看看

序列化数据的过程不应该是烦恼的

好的  开始动手吧  开发更好的游戏

我们讲解的还优雅吗




