## Devoxx 2014 Interviews: What's new in Android 5.0 Lollipop

![video_screenshot](images/l2-yvOmq5B4.jpg)

** 视频发布时间**
 
> 2014年11月27日

** 视频介绍**

> Chet (@chethaase, google.com/+ChetHaase) and Romain (@romainguy, google.com/+RomainGuygoogle.com/+RomainG-uy) discuss Material Design and other new developer features in Android 5.0 Lollipop.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 苏楚霖 | 高冰 | -- | [ Youtube ]( https://www.youtube.com/watch?v=l2-yvOmq5B4 )  |  [ Youtube ]( https://www.youtube.com/watch?v=lcXvjud0Suc ) | 1504260740 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

Alexis Moussine-Pouchkine: 大家好

这里是Devoxx 2014的现场  我现在与Chet和Romain在一起

你是Chet  你是Romain

还是你是Romain  你是Chet

ROMAIN GUY: 一样的

NICK BUTCHER: 是的

没关系

你不需要知道谁是谁

我们只是来聊聊Android 5.0的

你们对Android 5.0了解吗

CHET HAASE: 是的

知道

NICK BUTCHER: L代表什么

CHET HAASE: Lollipop（棒棒糖）


听上去不错

现在用户就能将系统

升级到Android 5.0

那新升级的系统都有哪些亮点呢

我现在走到哪都能听到

大家在谈论Material Design

CHET HAASE: 情况基本就是这样的

大家都在谈论Material Design

都在谈论Material Design是什么

如何实现Material Design的设计

ROMAIN GUY: 还有讨论别的

CHET HAASE: 有嘛

ROMAIN GUY: 有啊

CHET HAASE: 好吧

我最担心这个了

我所在的UI Toolkit团队

主要负责发布

与Material Design有关的消息

由于UX团队对Material Design的把握

太过于宏观

所以主要就由我们来让Material Design的概念落地

并要让大家明白怎样去实现Material Design

NICK BUTCHER: 有了你们的辛勤付出

开发者就可以省好多事了

CHET HAASE: 没错  不过这一点

要另说了

NICK BUTCHER: 那Material Design为开发者们

都带来了哪些新特性呢

我知道的有  新的配色方案

新的动画效果

并且这些新特性已经嵌入到系统平台内

CHET HAASE: 是的

是的

不过我觉得还有必要说一点

如果和别人聊了很多  看了很多有关Material Design的东西

你可能就会有疑惑了

在一大堆刚刚发布的API里

哪些才是要在应用中实现Material Design时能够用到的呢

答案是  其实并不多

很多资源都是免费提供的

当你选择了Material Design主题

或者你开始使用我们的设计依赖库

或者引用了appcompat包

那你就已经在开发基于Lollipop的应用了

而且会得到很多免费的

会为应用锦上添花的资源

这样你写出来的应用就显得更加规范

就像这个平台应该有的一样

而且  还有Material Design风格的动画效果  图标动态变化效果

控件的阴影和立体效果

这些东西也都是免费提供的

如果你不满于此  还可以自定义Material Design风格的设计

例如定制动画效果

或者activity跳转的效果等

开发一个应用不需要把我说的这些都用到

只是想表明在Material Design设计这条路上可以走多远

NICK BUTCHER: 好的

很明显Material Design会有大作为

用户都会看到它

开发者们也必须要知道

用户都希望看到些什么

ROMAIN GUY: 作为开发者一定要去阅读

Material Design的设计指南

在动画效果方面还有许多东西需要学习

NICK BUTCHER: 之前提到的这些

是为设计师准备的

还是码农们应该去学习的

ROMAIN GUY: 是这样

主要是面向开发者的  但对于设计师来说也一样重要

NICK BUTCHER: 涉及到的术语也是很重要的吧

可以让参与开发的人们步调一致

除了Material Design  肯定还有其他新鲜的东西

通知是一个能够立马显示在用户眼前的东西

为开发者准备的API里  通知会是一个什么样子呢

ROMAIN GUY: 锁定屏幕时能够呈现通知

是这次更新的一个新特性

用户可以选择允许什么类型的信息显示在锁屏界面上

因为我们考虑到了个人隐私问题

所以应用可以告诉系统

这些通知信息是属于公开的  私人的  还是保密的

用户可以决定

是否要公开某些私人信息

或是把所有一切信息都设为私人的

类似的设置还可以做很多种

CHET HAASE: 刚才说过有许多能够让应用表现更丰富的API

针对于通知这一部分

比如可将通知图标设置成各种色彩  来定制你的应用

或者对通知的样式进行一些细微的调整等等

NICK BUTCHER: 是的

你们所说的我们都有在关注

那目前所使用的与通知有关的API会有所调整吗

CHET HAASE: 他们都还能够正常使用

ROMAIN GUY: 是的

所有的API都可以正常使用

这看起来会很好

NICK BUTCHER: 确实不错

听起来很棒

并行文档

也是一个能够很直观展现给用户的东西

用户能够看到每一个他们使用过的应用

都以一个类似Chrome标签页的形式显示出来

目前是不是已经向开发者们提供了什么东西呢

ROMAIN GUY: 是的

我们提供了一个新的API

可以定义应用在概览列表里显示的文档样式

当应用新开启一个文档时

有很多可用操作

还可以规定在概览列表里应用要保留几个文档

在一些特定的应用  比如在doc文档应用或Chrome中

这一特性就显得十分有用

对于其他应用可能意义不会那么大

比如媒体播放器  音乐播放器就是这一类

不过这完全取决于开发者

NICK BUTCHER: 我在新版本介绍中还看到一项

就是Android 5.0包括了一个适用于WebView的Chromium版本

自KitKat版本以来WebView已经开始基于Chromium

现在更新后的WebView包含了一些新特性

WebView变成了独立的部分

它不会跟随系统更新一并升级  是这么一回事吗

CHET HAASE: 是的  WebView可以从Play商店中获得更新

NICK BUTCHER: 直接在Play商店发布更新

CHET HAASE: 是的

WebView现在已经可以从Play商店获得更新

所以你再也不用守着新系统发布的日程表

苦苦等待WebView的更新了

现在随时都可以获得WebView的更新

NICK BUTCHER: 也就是说

比如Chromium对WebGL的支持有提升等这类更新

我们很快就能获取的到

ROMAIN GUY: 是的  不过及时获取修复bug的更新显得更重要

NICK BUTCHER: 那是当然

CHET HAASE: 是的

不过我并不知道这一特性实施的详细方案

比如我不知道在Play商店更新WebView的频率

不过在发布更新时一定会在系统架构和性能方面做足准备

确保之后可以在Play商店发布单独更新的版本

NICK BUTCHER: 太好了

那再来聊聊其他的API

我想了解一下与Runtime有关的内容

ROMAIN GUY: 那有太多API了

NICK BUTCHER: 是的

听说有5000个

有点吓人哦

但我们没有时间说其中的4900个

在剩下的100个里有没有想向我们介绍的API呢

ROMAIN GUY: 让我想想看

我来说一些我个人比较喜欢的API吧

比如有可以支持运行PS1的API

我觉得这对很多应用都很有用

但很明显并不是对所有应用都有用

我当然也很喜欢标准统一的播放控制API

用它可以来控制音乐的播放

现如今在通知界面上有各式各样的音乐控制窗口

因为每一种播放器应用

都各自为营

这可能给用户带来了一些困扰

但这就是目前普遍的现状

不过既然应用可以定制自己的通知样式

它们会更像是个人的音乐应用

这对于用户来说还是挺方便的

NICK BUTCHER: 那再说一个你们可能会感兴趣的

这次也更新了对OpenGL的支持  对吧

这次都更新了哪些东西呢

这次只是一次普通的OpenGL版本更新吗

ROMAIN GUY: Android 5.0现已经支持OpenGL 3.1了

这给图形工程师和游戏开发者

带来很多有趣的功能

并且还推出了

Android扩展程序包 (AEP)

它将20种OpenGL引擎

扩展程序集合在了一起

我们保证这些扩展程序

都会包含在Android 5.0的设备里

这样更方便管理

NICK BUTCHER: 那这些东西

其实都是基于新的运行环境了

目前ART是唯一的运行环境了

你们不会再返回使用Dalvik了吧

ROMAIN GUY: 不会再回去了

CHET HAASE: 我猜  用过ART和Dalvik的人都会说

ART是一个更好的运行环境

ART采用提前编译的方式

有更好  更快  更高效的垃圾回收机制

对象的分配和回收也变得

更加快速

作为一个灵活的垃圾收集器

堆栈的碎片整理将会更加高效

当activity在后台运行时

正是ART垃圾收集器

运行的最好时机

它会给堆栈腾出更多的空间

这在Dalvik中是做不到的

NICK BUTCHER: 有了ART是不是就可以

实现60帧率了呢

CHET HAASE: 是的

是的

分配的对象越多  就会产生越多的垃圾

过了一会儿  垃圾回收器可能会说

我需要释放更多的内存

由于目前没有足够的内存

所以垃圾收集器会去回收那些无法被引用到的对象

以此来创造出更多的可用空间

但是这样做就会占用越来越多的时间

堆栈中的碎片越多  ART要做的事情就越多

从而就会看到卡顿现象

如果开启了日志打印

就会看到  当让运行的所有程序都暂停进行垃圾回收时

一般卡顿时间都会在10到20微妙

有了ART之后  卡顿时间可以降低至2到3微秒

也就是说

ART足足节省了16微秒

这16微秒足以

将所有像素信息渲染出来了

从而保证了60帧率

这对动画或者其他类型的渲染都很重要

如果我们能够解决卡顿带来的问题

让每帧的渲染时间不再那么长

那我们就能轻松的做出

流畅的画面

NICK BUTCHER: 如果人们对

垃圾回收机制感兴趣

我推荐他们观看Google I/O大会的视频

在那里可以获得更多的细节

CHET HAASE: 收听Android Developers Backstage播客也可以学到很多

由于我讲Runtime时太投入了

我们跟Anwar聊的时间超出了预期  就把播客内容分成了两部分

NICK BUTCHER: 实际上我两部分都听了

CHET HAASE: 是吗

NICK BUTCHER: 我对这个十分感兴趣

所以听完了第二部分

我也建议大家去听一听

让我们再来看看用Project Volta查询耗电量信息

它现在是停留在

内部项目阶段

还需要收集和分析数据

还是已经向开发者们开放了

ROMAIN GUY: 这有点类似于我们之前的项目

Project Butter和Project Svelte所做过的事

他们都属于内部项目  用来收集数据

以便去了解Android系统到底是如何运行的

并修复一些已知的问题

然后制作出可用的工具

供开发者们使用

这就是所谓的Battery Historian

它被托管在了github.com/google上

这也是Android团队发现问题时所用到的工具

CHET HAASE: 实际上有很多工具

跟在Android上看到的工具很相似

一些工具看上去摆不上台面

但它们就是这么有用的存在着  不是吗

比如在移动设备或者DDMS里

的一些GPU分析的工具

之所以存在是因为大家需要它

来多方位地了解Android

比如我需要一个工具

可以向我展示一些有用的信息

你就动手编写出了这个工具

那就没理由不让别人

也受益于这个工具

NICK BUTCHER: 好的

你提到的东西

有的我不太了解  这是你自己喜欢的功能还是什么

我觉得像是在选择什么

ROMAIN GUY: 我想说Android 5.0是一个大的更新版本

我认为每个人都应该了解一下

可以在模拟器上面运行一下Android 5.0

各种设备上的系统镜像也都可以很方便获取到

或者可以看看新版本的介绍

我觉得每个人都可以从中受益

NICK BUTCHER: 是的

我们今天没有讨论硬件设备

不过确实有一些令人眼前一亮的设备让我们不得不关注一下

手机  平板等  作为用户能够第一时间上手

这感受是最棒的

对于开发者来说

这也都是非常酷炫  非常强大的设备

还有其他想说的吗

CHET HAASE: 动画效果

很多新的动画效果

这总归是件好事  对吧

ROMAIN GUY: 这是你所关心的吧

CHET HAASE: 当然

好吧

好的

好吧

NICK BUTCHER: 那好

今天我们就聊到这里了

谢谢两位

ROMAIN GUY: 谢谢

CHET HAASE: 谢谢

NICK BUTCHER: 再见

再见各位