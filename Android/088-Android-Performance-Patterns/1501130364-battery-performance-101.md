## Android Performance Patterns: Battery Performance 101

![video_screenshot](images/9i1_PnPpd3g.jpg)

** 视频发布时间**
 
> 2015年1月6日

** 视频介绍**

> Battery is the most precious resource to Android users right now. The world is more mobile, but it’s frustrating when you can’t make it through a full day without needing to recharge your phone. And Sadly, for most developers, Battery Efficiency is the last thing on their minds.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 周亿 | 姜昭宇、Kesen | —— | [ Youtube ]( https://www.youtube.com/watch?v=9i1_PnPpd3g )  |  [ Youtube ]( https://www.youtube.com/watch?v=9i1_PnPpd3g ) | 1501130364 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

电量其实是目前手持设备最宝贵的资源之一

但是很可惜  大多数设备都需要

不断的充电来维持继续使用

不幸的是  对于开发者来说

电量优化是他们最后才会考虑的的事情

我是Colt McAnlis  但是可以确定的是

千万不能让你的应用成为消耗电量的大户

使用几个简单的API和工具

你就能够做出一个快速的

很赞的  被用户喜爱的应用

让我们后退一步

现阶段的电池使用到底有多糟糕呢

Purdue University研究了

最受欢迎的一些应用的电量消耗

结果令人震惊

平均只有大约25%到30%左右的电量

是被程序最核心的方法例如绘制图片

摆放布局等等所使用掉的  或者是发射愤怒的小鸟

剩下的75%左右的电量完全是被上报数据

检查位置信息  定时检索后台广告信息所使用掉的

这个发现为开发者提供了一个有趣的问题

不难发现  这些应用程序实际上

只给用户提供了些许花边功能

但却是以用户的电量为代价滴

迟早用户会因为这个性价比而不满意这个应用程序的

聪明的开发者致力于寻求两个极端之间的平衡

他们发现能够使用更少的电量来实现操作

我们应该尽量减少唤醒屏幕的次数与持续的时间

使用WakeLock来处理唤醒的问题

能够正确执行唤醒操作并根据

设定及时关闭操作进入睡眠状态

同样的  某些非必须马上执行的操作

例如上传歌曲  图片处理等

可以等到设备处于充电状态

或者电量充足的时候才进行

网络也是电池的另一个大消耗点

触发网络请求的操作

每次都会保持无线信号持续一段时间

当然  仅仅是等待也是耗电的

我们可以把零散的网络请求打包进行一次操作

避免过多的无线信号引起的电量消耗

你就会每隔五秒一次又一次进入等待

还好Android有几个工具能够帮助你

追踪并解决这些电池问题

首先  我们可以通过手机设置选项

找到对应App的电量消耗统计数据

然后选择你感兴趣的应用

你可以看到屏幕上的数据报告

告诉了你设备处于唤醒状态的时间

是否有网络连接

想要更深入的进行分析

你可以通过Battery Historian Tool

来查看详细的电量消耗

一旦你找到了问题所在

Android有几个API能够帮助你修复它们

举个例子  如果发现我们的App

有电量消耗过多的问题

我们可以使用JobScheduler API

来对一些任务进行定时处理

例如我们可以把那些任务重的操作等到手机处于充电状态

或者是连接到WiFi的时候来处理

如果你是在寻找更精妙的使用电池的方法

来为你的用户节约宝贵的电池资源

记得查看Android Performance Patterns

的其他视频

代码分析  你值得拥有  性能问题  永不能忘




