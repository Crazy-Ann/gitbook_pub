## Under the Hood of Android Auto 

![video_screenshot](images/KNKGM4ss5Sc.jpg)  

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> Your car contains some serious technology. Learn about the Android Auto architecture, which enables you to control Android apps and services running on your phone through your car. In this talk, we'll highlight the key characteristics of the Android Auto protocol, which enables your Android phone to talk to compatible cars. We'll also take a look at some of the details of the Android Auto rendering subsystem, which uses Binders and the Android VirtualDisplay API to composite UI from multiple Android apps. Finally, we'll discuss how we're enhancing the Google Maps app by integrating with the Android Auto platform.

** 视频推介语 **

>  暂无，待补充。

### 译者信息 

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| 黄莘 | 卢治泷 | -- | [ Youtube ]( https://www.youtube.com/watch?v=KNKGM4ss5Sc ) | [ Youtube ](https://www.youtube.com/watch?v=bVRRll6McjI) | 1504020501 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator ) |


### 解说词中文版：

FABIAN TAMP:  大家好  我是Fabian

我是一个Android和Google Maps团队的软件工程师

我的团队致力于让

你喜欢的Google Apps在你的汽车上也能使用

并且我们对于Android Auto很激动

因为它把你汽车上最后的硬件和

你的Android手机的可升级性，连接性

以及个性化设置全都联系到了一起

你的汽车目前是最复杂的附件

有史以来用在Android手机上的最复杂的一个

它有一堆传感器

以及视听识别功能

让我们从Android Auto的协议开始聊起

这个协议使得你的手机可以和汽车进行交互

这个架构的最大特点之一

就是Android的应用和服务全都运行在

你的手机上同时在你的汽车上控制使用

我们把应用压缩在一个视频流

和音频流之中并且把他们发送到汽车中控单元

通常来说  汽车的更换周期更久

并且汽车中的软件更新的比智能机中的要缓慢很多

所以通过把运算和渲染过程转移到手机上

我们能利用了最新的手机技术的优点

并且保持你的Android Auto体验

在你的汽车的生命周期中始终与时代同步

我们想使得Android Auto的协议是非常容易与

汽车组合到一起的  所以给制造商提供了一个轻便的

C++库  这个库是运行在汽车的中控单元里的Linux，Android

以及QNX系统之上的

这个Android Auto协议使用的核心思想

就是把通道按优先顺序区分好

不同的通道是给你的汽车不同的方面开放的

这个是手机需要联系的

通道是对音频  数据展示 用户输入 位置数据 开放的

比如GPS和轮子转速

这些通道通过USB连接多重传输

这个USB连接是支持

这允许我们给那些影响用户体验最大

的通道优先权

我们已经在Android Open Accessory协议之上创建了这个Android Auto协议

但是它被设计为传输形式不可知的

这样我们能够基于其他的连接形式开放它

比如在未来的Wi-Fi直连

为了格式化数据  我们广泛地使用了protocol buffers

protocol buffers是一个开源的Google技术

这个技术使得未来加入新特性特别地方便

同时得以维护以前版本的稳定性

一个我们的关键的设计目标

是使得Android Auto感觉起来像完全融合进你的汽车里面了

在第一个版本中  我们得到不同的输入

方式的支持  特别是触摸屏

以及硬旋转控制器  在一个相似的方式下

来规则的Android UI支持触摸

以及控制器的模式

我们也支持把指令发送到

仪表盘控制器上  这样可以展现他们以及

当他们可获得的话与你的方向盘的按钮一体化

我们也支持音频路由给不同的在汽车中的音响

在以音频的类型为基础

举个例子  在Google Now中的旅行建议

现在可以仅仅只对于驾车的人

同时音乐的播放是可以被汽车中所有人播放的

总是会有这样的时候  举个例子

当你在收听广播的时候并且想去问Google Now来读一个信息

的时候

所以汽车和手机以类似Android手机上APP之间

相似的协商方式来协商音频的关注点

那个汽车有一个基本申明  关于什么时候Android Auto是可见的

或者什么时候播放音频   这样他可以保证重要的安全提示

以及倒车摄像机是优先的

在手机的一端   我们正在Google Play服务中建设

Android Auto代码  所以你的体验可以是最新的

Android Auto系统广泛地使用Android视觉

展示API

让我们深入下去以及看一下这个渲染系统

在Android Auto中  通过应用过程

的边界展现在一个一般的汽车屏幕上

我们使用XML来确定一个窗口的展示

是被很多不同的应用渲染成功的

这有一个窗口包括了旅行线路

主要信息区域   提示区域

以及一个搜索区域

任何一个窗口事实上是一个android.view.TextureView

Android Auto服务让TextureViews回到

SurfaceTexture  把它包裹在一个表面对象中

并且把它通过二进制接口传输到一个

客户端线程

在客户端的库中  一个私有的视觉展示

被表层给创造出来   并且应用的UI

在扩大在视觉展示上

我们之后致使XML展现通过另一种视觉展现来压缩多页面

这个是被手机硬件视频编码器支持的

然后把内容输出到汽车中控单元

在这个架构背后  有两个核心原则

第一个是灵活性

在XML展现中使用TextureViews

使我们能够任意地展现窗口

这个意味着我们可以利用完全的Android展现系统

包括动画

第二个是安全以及稳定性

通过控制客户端维持在他们自己过程中

我们能把问题从系统中的其他部分孤立出来

并且保证应用没有任何权限去接触他们不能接触的数据

同时  我们也想保证手机上现存的应用

可以利用汽车中可获得的

经过优化的位置信号

所以我们已经把这些信号融合进Google Play服务的


这个Fused Location Provider把智能手机上能使用的

不同位置技术融合起来

比如移动信号  Wi-Fi 以及GPS

这些技术被融合进一个简单高级API  而这个API允许开发者

制定精度要求和更新频率

而不是与单独的位置源进行交互

通过从汽车中加入位置源数据

我们正在增强位置数据的精确度通过使用

应用正在使用的API

所以现在  我将要告诉你有关

我怎么使用Android Auto以及Google Maps应用

来增强汽车内的体验

首先  Google Maps对于导航是更加的简单的

当它投放在一个大的屏幕的前端中心

而不是在一个你的仪表盘上的

小的手机屏幕

我们已经重新设计了Maps来很好地

工作在一个水平方面  并且充分使用了用在汽车上的UI

举例来说  通过减少任务结束时间

以及通过使得触摸目标容易被触碰到

汽车上的Google Maps的众多最大的好处之一就是

使用Fused Location Provider

我们可以使用你汽车中的GPS信息  举例来说  

这个将会非常大地提高在城市中驾车的位置质量

我们也可以使用你的汽车罗盘  陀螺仪  车轮速度

以及其他的位置传感器来算出

你正在面对哪条路  以及你已经在

隧道里穿过的确切距离

所有的这些使我们能够给你们更加多的

准确的驾车指南来让你有更少地阻碍开到你的目的地

所以这就是一个Android Auto如何在你的

Android手机以及你的汽车中使用的技术的一个大概描述

以及有关创造一个美好的驾车体验

我们对于Android Auto将要在

汽车内的娱乐以及旅行更在无缝更在联系更在安全

创造出的可能性而非常激动

谢谢观看

