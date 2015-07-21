## NFC + HCE Your phone in an interactive world 

![video_screenshot](images/ZaVkKagA_oA.jpg) 

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> Host card emulation is gaining steam in the Industry with Visa and Mastercard now backing the technology for Mobile payments. Since KitKat, when HCE was introduced with little fanfare, we've gotten inundated with questions and guidance from large firms across multiple industries. Many want to know what we are trying to to with NFC/HCE, how we're looking to position the technology, and how they can leverage it in their use cases. Interested parties range from building access, loyalty programs, payments, mass transit, airlines, banking, etc.This would be a great opportunity to highlight how we came about with our approach for HCE, as opposed to an embedded secure element approach, why we think its great and how people get get started making applications now that large players have thrown their hats into the ring.

** 视频推介语 **

>  暂无，待补充。

### 译者信息 

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| 黄莘 | Wallace4ever | -- | [ Youtube ]( https://www.youtube.com/watch?v=ZaVkKagA_oA ) | [ Youtube ](https://www.youtube.com/watch?v=EcmKIZjzP_8) | 1504020509 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator ) |


### 解说词中文版：

嗨

我是Andres 我来自Android NFC团队

我很高兴能在这里和你谈论全新伟大的NFC

和HCE功能  而这些功能我们已经

为AndroidL开发者预览版进行了开发

首先  让我们来看看HCE是怎么回事

以及我们如何使它在Android L开发者预览版中表现更好

在Kitkat中  我们使用HCE供应NFC无线电

开放NFC的非常简单的接口

来适应任何设备上的任何开发

NFC应用都不再被强制在

专门和特有的硬件上运行

而现在NFC应用可以在CPU上直接运行

这使应用程序可以在任何KitKat或更高版本的设备上运行

以此来利用日益发展的NFC生态系统中的功能

例如轨道交通  身份  建筑访问这样的

都是你可以使用HCE

建立的冰山之一角

HCE使您的手机上的应用程序看起来像一个智能卡

如公交卡或支付卡

就像一个运行在智能卡上的应用程序

一个HCE应用程序只需要注册一个应用程序标识符或AID

应用标识符允许NFC阅读器

选择他们想要交互的应用程序

例如  我们的I / O传输的应用程序

在Android运行时能够注册它想要的AID

当你点击你的手机的传输阅读器时

通过选择AID  I / O传输的应用程序

得到了自动调用

之后它自由地与阅读器交换任意数据

根据您的反馈  我们已经提升HCE的能力

使它符合更多的使用案例  更易于集成

并且在Android L开发者预览版提供广泛的可用性

让我们来看看有什么新的内容

很多HCE的早期开发者注意到

他们在编译的时候不知道他们的AID清单

他们希望根据它们的应用程序的状态

使用动态的方式注册它们

从Android L开发者预览版开始

应用程序不需要在清单中静态注册他们的AID。

现在 应用程序可以在运行时

为它们感兴趣的AID进行动态注册

例如  如果你的会员卡

接收到一个新的会员卡类型具有不同AID

你可以注册它而无需重新编译应用程序

使用这些API动态注册您的应用程序的AID

我们也提升了应用程序在前台

处理事务时的可能性 甚至是在应用程序可能不是

那个AID的默认应用程序的时候也是如此

在KitKat中  你只能选择一个应用程序

来处理你所有付款事务

这将迫使用户进入设置切换默认的应用程序

Android L开发者预览版可以让你的

应用程序在前台时  对于一组AID注册为

临时默认的应用程序

想象一下  你有一个只能在你的商店使用的支付应用程序

就叫它OneStorePay好了

可能它不会被设置为默认的支付应用程序

但是  如果用户打开你的应用程序  在她点击之前

该交易是由你来处理的

该个叫作AllStorePay的应用程序可以在每家商店中使用

将就像用户期望的那样工作

当你的应用程序不是在前台时

你其实已经使用了这些API来注册您的应用程序

以进行动态前台调度了

你可以找到更多有关如何编写HCE应用程序的支持  以及

我们所有了不起的的新功能 

谢谢你今天能够抽出时间看我的讲话

希望看到你能尽快开发出全新而且很棒的NFC和HCE应用程序

