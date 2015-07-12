## Android Performance Patterns: Tool - Memory Monitor

![video_screenshot](images/7ls28uGMBEs.jpg)

** 视频发布时间**
 
> 2015年1月6日

** 视频介绍**

> During the lifetime of your application, You can expect the amount of allocated memory to change quite frequently. For example, needing to allocate more bitmaps for your social media data;Or plotting a new jogging path that takes your user past a trendy donut shop. What’s tricky though, is seeing how these allocations, can impact your performance.In this video +Colt McAnlis, introduces a fancy tool in Android Studio, which lets you can get a better sense of how your application is using memory.Watch more Android Performance Patterns here: http://goo.gl/3dBbse

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 周亿 | 姜昭宇 | —— | [ Youtube ]( https://www.youtube.com/watch?v=7ls28uGMBEs )  |  [ Youtube ]( https://www.youtube.com/watch?v=7ls28uGMBEs ) | 1501130363 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

在你应用程序的生命周期中 

你能看到很多关于 

相当频繁的内存分配 

比如  在你的社交流媒体应用中 

加载一个或多个位图 

或者是增加一条新的慢跑路线 

并带你的用户去一个新的时髦的甜甜圈店 

让我们来看看如何通过合理的分配来 

提升你的应用程序的性能 

我是Colt McAnlis 

在Android Studio里面有一个 

新的时髦工具能够帮助你更好的理解 

你的应用程序是如何使用内存 

它能够帮助你赶在用户开始注意到之前 

发现任何内存分配相关的性能问题 

使用Android Studio里面的新的 

内存监视工具能够让你解决这些问题更容易一些 

这个工具能够给出一个快速的图形概览 

让你知道你的程序在一段时间内的内存使用情况 

在窗口的左上角 

你能看到当前链接的设备 

在右边选择你想要监控的应用程序 

如果你有多个设备或者程序正在运行 

你可以在这进行选择 

在窗口的中部的图形是堆栈图 

其中  深蓝色的显示的是 

你程序当前使用的内存数 

上面的浅蓝色是系统 

分配的可用内存 

这个图会不停的变化  更新 

来展示出内存使用的变化情况 

现在  假设你的应用没有做太多的事 

那么你看到的应该是像这样的平坦的曲线图 

从性能的角度看 

这实际是一个理想的方案 

随着你的应用分配和释放内存 

你会看到图形在同一时间内的 

内存分配的大小的变化 

任何时候  你分配过的内存突然急剧下降 

那么垃圾回收事件收到了回收的指令并执行完成 

这些垃圾收集事件不算什么大问题 

但是  它们在短时间内大量反复进行垃圾收集 

就会导致许多的性能问题 

你用来收集垃圾的时间越多 

你用来干其他事情的时间就越少 

比如渲染  或者音频流处理 

要启用内存监视器 

打开Android Studio 

连上你的物理设备 

然后运行你的应用 

然后在工具菜单中选中内存监视器 

一旦监视器运行 

在屏幕底部的新标签会显示所有相关信息 

虽然内存监视器会告知你 

大体的系统性能和健康状况 

但是它不会帮助你追踪任何有关的问题 

要想做到追踪  你需要一些更强大的东西 

比如堆内存工具 

它能够帮你找到你代码中 

哪里有创建了但是没有释放的对象 

它会对创建了但是没有使用的对象 

或者是你能重用 

但是却创建了新的的对象进行处理 

虽然Java的内存自动回收机制 

让你对于内存的管理很方便 

但它还是需要做很多的工作 

才能保证让你的应用程序以最快的速度运行 

这也是为什么你需要查看 

本系列的其他视频 

来学习更多关于内存使用的技巧和窍门 

当然别忘了加入Google+的讨论组 

这样你就能从其他的开发者那得到宝贵的建议 

代码分析  你值得拥有  性能问题  永不能忘 




