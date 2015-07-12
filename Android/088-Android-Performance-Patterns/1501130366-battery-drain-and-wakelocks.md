## Android Performance Patterns: Battery Drain and WakeLocks

![video_screenshot](images/reMau7d0yeg.jpg)

** 视频发布时间**
 
> 2015年1月6日

** 视频介绍**

> It’s no secret that in order for your app to be successful, the user has to run it. And for it to continue to provide value, sometimes it needs to keep running. But this is tough to do while the phone is sleeping. But the answer is simple right? Just wake it up and do the work! Maybe, but tread lightly here…. there’s a massive battery problem waiting to happen.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 周亿 | 姜昭宇、Kesen | -- | [ Youtube ]( https://www.youtube.com/watch?v=reMau7d0yeg )  |  [ Youtube ]( https://www.youtube.com/watch?v=reMau7d0yeg ) | 1501130366 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

众所周知  如果一个应用程序想要获得成功

就要有用户来使用它

而且为了能够持续为用户提供服务

有些时候可能会需要后台运行

但是当手机是休眠状态的话就有点不开心了

我的意思是  如果用户的手机已经休眠

你要把它唤醒才能去做点什么

这是真的  这不是梦

但是这里隐藏着一个巨大的耗电问题

我是Colt McAnlis

手机休眠状态下持续被应用打扰

这将会消耗更多的电量

但是只要一点点小的改动

你就能以更小的电耗达到相同的目的

为了说明这一点

我拿我的好盆友Rado举个例子

他是一个社交达人  游戏玩家

也就是说他要运行的手机程序

基本都是比如检查积分榜

上传照片  不停的上Twitter刷新

标签#crazes查看内容

这些应用程序在Rado手机休眠状态下还在继续跑

于是乎才到了午间十分  他的手机就么有电啦

Rado不得不给手机不断充电

这都是手机没有休眠造成的

也就是说  这些应用程序不断地唤醒手机

它们缩短了电池持续续航时间

而不是让手机好好休眠  而休眠是很重要的

Android系统会关掉部分硬件来节约耗电

首先  屏幕变暗

然后完全关闭  之后CPU也进入休眠

这一切都是为了节省宝贵的电池资源

即便在这种非活跃状态

大多数的程序也会尝试通过唤醒手机的方式继续工作

唤醒手机最简单的办法是用

PowerManager.Wakelock API接口

它会保持CPU运行  防止屏幕变暗或者关闭

这样你的手机就能在未来某一时间唤醒

做一些工作  然后在接着休眠

最后  也是最微妙的一点

使用Wakelock非常简单

难的是怎么去释放它

掉坑的方式有很多种

但是如果在上传到服务器之前

你的应用需要花60分钟而不是10秒来分析这些图像

或者是服务器跪了

你永远也得不到社交媒体的响应

难道应用程序就应该苦苦等候么

结局就是  手机一直没有休眠  一直在耗电

这时候  你就可以使用

wakelock.acquire外加一个超时参数

它会在一段时间里强制让Wakelock释放

以防上述事件发生

但是这也不能完全解决问题

那么  多久才算超时呢

第一次超时之后  等待多久再次尝试呢

正确的解决方案是使用非精准定时器

通常情况下  你设定了一下时间来触发事件唤醒手机

但是最好改一下这个时间  以便节省电量

例如  如果有另外一个程序需要

比你设定的时间晚5分钟唤醒

最好能够等到那个时候

两个任务捆绑一起同时进行

这就是非精确定时器的核心工作原理

我们可以定制计划的任务

可是系统如果检测到一个更好的时间

它可以推迟你的任务  以节省电量消耗

在现实世界里  有很多情况下

都可以节省电耗  比如充电时

连接WIFI时  抑或是设备

被另外一个进程唤醒的时候

如果你把任务都安排在上述情况下进行

那么就可以显著的提高电池寿命

这正是JobScheduler API所做的事情

它会根据当前的情况与任务

组合出理想的唤醒时间

例如等到正在充电或者连接到WiFi的时候

或者集中任务一起执行

我们可以通过这个API实现很多免费的调度算法

不要忘记用户已经可以看到每个应用程序的耗电情况了

并且可以在该界面直接与你的软件说拜拜了

也就是说你也许应该花一些时间用

Battery  Historian工具来看看

你应用程序的唤醒逻辑是否合适咯

这个工具随着Android L发布了

它可以在一个漂亮的界面查看程序被唤醒的频率

由谁唤醒的  持续了多长的时间等等

有了这些新的工具和接口

你应该可以让手机的休眠时间得到充分保障啦

还有  如果  你想避免设备休眠

那么去查看Android Performance Patterns系列视频吧

同样别忘了加入G+社群与我们沟通

代码分析  你值得拥有  性能问题  永不能忘