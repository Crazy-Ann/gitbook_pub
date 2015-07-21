## An Introduction to Android Wear

![video_screenshot](images/Bl4Qne-RpcM.jpg)

** 视频发布时间**
 
> 2014年6月18日

** 视频介绍**

> Timothy Jordan gives an overview of the Android Wear developer preview back in June 2014. Since that time, the platform has been made available to all developers, many watches were made available for purchase, and even custom watch faces are now possible! For the most recent information on the Android Wear platform, please visit http://developer.android.com/wear.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| Guangwei Feng  | 點墨 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=Bl4Qne-RpcM )  |  [ Youtube ]( https://www.youtube.com/watch?v=wH3EZO0ChbA) | 1503190435 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

TIMOTHY JORDAN: 大家好，我是 Timothy Jordan.

我在Google负责开发者技术支持工作

今天给大家简单介绍一下Android Wear(Android可穿戴设备).

Android Wear是对Android平台的一系列API扩展

用来支持全新的可穿戴设备

(通过这些API)可以让各种各样的提示信息显示在可穿戴设备上

而不需要改变现有的Android app代码结构

开发者只需要添加很少的代码

就能扩展App在可穿戴设备上的体验

或者更加深入一点 开发一个可穿戴设备专属的App

在深入(Android Wear)平台的细节之前

我们先来看这样一个问题

这场景有什么问题

我们研究科技产品的使用情况

寻求各种方法

在让人们更多地接入数字世界的同时

也能多多参与身边的事情.

Android Wear能够实现以上的期望，

在你正好需要的时候，展示给你关键的信息，

而且仅仅只需要一瞥的功夫

让我们从更技术性的方式看一下

这是我们一天里对手机的使用

注意各个时段消耗的时间

从口袋里拿出你的手机

解锁，选择你需要的功能，最后才是使用

这耗费了大量的时间和精力

甚至一些本来需要很短时间的交互(也是如此)

这是同样的交互在可穿戴设备上的时间消耗情况

注意在每一个交互上的时间消耗的减少

这就是我们所说的更关注现实世界

同时更加连接虚拟世界

这些对开发过程有什么意义呢

首先，有一点非常重要

Android Wear采用了从底层改变的用户交互模型

注意这台设备，你就能够发现

它和其他移动设备是完全不同的

(所以)为了真正确保用户体验

我们必须重新思索它(的特性)

对于一个服务  想要确定哪些特性要在手腕上实现

首先考虑这样一个问题：

什么功能是我们之前不可以在手机上完成，但是现在却能在手腕的设备上实现的？

什么(新特性)现在成为了可能？

然后我们就可以重点关注这些

而且去尝试(实现）它

这听起来似乎有些开玩笑，但是当你拿起了你的(Android Wear)模拟器，

运行它，站起来在桌子边，

然后假装你在不同的会议之间行走，或正在穿过街道，

或者是其他不同的场景下

你就能知道在行进中使用移动服务是什么感觉

接下来是用一个很简单，但是有很必要的不同的实例

来展现我们的想法

这是手机上的App体验

我们现在已经让用户习惯了把这些App都放到一块儿

然后在需要的时候在这里面去找

这样的操作在手机上是没有问题的

但是，如果我们把同样的图标模式放在一个穿戴设备上，

这就不怎么合理了。

在想要减少这部分交互的设备上

这同样是很耗时的

所以,(之前的模式)很不合理

那么，我们应该如何跳出这个旧的流程呢

我们该如何越过充满图标的网格呢

这是Android Wear的用户界面

非常简洁，可以在一瞥内获取信息，而且只需要极少量的交互

用户交互被分为了两种主要的方式

首先，用户可以使用语音和设备交流

你可以把这些当做”用户操作”

用户可以说句”OK Google”

然后就可以使用其他语音命令(操作设备)了

其次，设备也可以把信息传递给用户

让我们把它当做一个内容流

填充了众多增强版的提示(Notification - Android提示栏信息)

而且是当时对用户最关键的(提示)

因为它出现在最正确的时间和位置


让我们来关注一下Android Wear的开发

首先，是各式通知(Notification类)

手机上的通知也会展示在穿戴设备上

对此你不需要额外做任何工作

它是自动完成的

同样，不论是在其他设备，例如手机，还是在可穿戴设备上

提示都可以振动或发声

增强版的提示也能显示在可穿戴设备上

同样，实现这些功能你任然不需要做任何额外的工作

它也是自动完成的

你还可以针对可穿戴设备

对你的提示做很多的定制

当然，这些需要多一些的代码
栈(Stack)允许你把众多提示叠在一起

就像收件箱那样 

页面(Pages)

它们能在一个提示中

展现比”一瞥”更多的内容

当然，页面(Pages)可以和栈(Stacks)联合使用

回复(Replies)

回复允许你给提示添加更多用户动作

让用户可以用自己的语音操作设备

来输入开放式的文本或者提前定义好的内容

如果你想要让自己的代码运行在可穿戴设备上

你需要搭建一个Android Wear App

虽然Android Wear的SDK尚未发布（翻译时已正式发布和提供免费下载）

但是下面几条描述可以帮助你提前构想

你可以自定义卡片布局

然后在穿戴设备上运行activities(Android Activity类)

你可以通过调用数据复制API和远程过程RPC

在手机和设备间传递数据和操作

你也可以收集传感器数据

然后实时展示在设备上

你可以注册你的app

让它能够响应语音操作，就像”OK Google,take a note“(Android Wear源生暂不支持中文语音输入)

以上便是Android Wear平台的快速介绍

请登录下面的链接获取更多相关文档和说明

developer.android.com/wear.(需科学上网)

我是Timothy Jordan,我们下次再见。
