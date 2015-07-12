
## Coffee with a Googler: Chat with Francis Ma about Google Play services

![video_screenshot](images/sMAv9RKlHjE.jpg)

** 视频发布时间**
 
> 2014年12月19日

** 视频介绍**

> Google Play services is a set of APIs that let you build better apps. From maps and location services to monetizing your app with wallet or ads, it's got everything you'd want to be the best mobile developer you can me. In this episode, we'll down some joe with Francis Ma, product manager for Google Play services, and who just happens to be a really nice guy!

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 鲁登科 | 周亿 | -- | [ Youtube ]( https://www.youtube.com/watch?v=sMAv9RKlHjE )  |  [ Youtube ]( https://www.youtube.com/watch?v=sMAv9RKlHjE ) | 1501120028 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

欢迎来到谷歌园区

在我来这里工作之前

我一直想着能来谷歌园区

并且和Google工作人员一起喝咖啡

聊聊他们在干些什么  怎么做的

和为什么这么做

今天我们会请Francis Ma来一起谈谈

他是Android团队的一位产品经理

他会告诉我们怎么通过Google Play services

做出更好的程序

Francis  非常欢迎

很高兴你能来这儿

谢谢  Laurence

我也很高兴坐在这儿

有一件事我要说的是

当我们正在准备这个节目的时候

每次我告诉其他Google工作人员

我们请到了Francis Ma来做嘉宾时

他们都会说  天啊  你请到了Francis Ma

我和他在一个项目  我和他一起工作

看起来你涉及面很广

告诉我们你在做什么吧

好的  我已经在Google工作两年了

我有幸参与了不同的产品研发

最近的一次 在加入Android之前

我在Google+团队中参与社交应用

太酷了

听起来太有趣了

是啊  当然

非常有意思

现阶段

Google Play services是你工作的一部分

那么Google Play services到底是什么呢

它是干什么用的

到底哪里让它那么炫呢

Google Play services是用统一的SDK开发的

那是我们提供给开发者的一种方式

可以与Google services和Google APIs联系起来

你说那是一种统一的方式

他们可以使用这种服务和API

怎么来统一呢

方法是这样的

如果你是开发者

你可以申请一个Google Play services的SDK

然后你就有各种Google平台的API的权限

那是我们提供的就像Google Ads


Google Wallet等等

因此这种设计模式是

我编写代码时遵循的

就像Google Maps

Google Wallets和Google Ads

我都因此使其一样

很显然

这是Google Play services的设计理念之一

在一开始的时候

我们就想给Android开发者提供始终如一的体验

可以将各种各样的产品特点和

Google提供的功能整合起来

例如  如果你和Google Maps关联

然后你又选择与Google Analytics关联

相同的的模式和规则

是非常一致的

可以让我们不用再学习完全不同的东西

并且便于你再在你的程序中添加

那太酷了

如果我学会了在程序中使用Maps的方法

然后我想要把这个方法应用到--

我也不确定什么地方 如果我想要使用定位的话

这真的是酷毙了

我喜欢

但是你的一个词突然引起了我的思绪

那就是开发经验

开发经验

在Google中是十分重要的

这也是你特别热衷的东西

你可以告诉我们一些关于它的东西

和你在这方面做的事吗

当我们着眼建立API上时

我们是将它当做一个产品

以此类推的话  如果你使用一个客户端

我们会看看它的视觉设计

和它的用户体验

就像下载程序和安装程序之类的

什么是onboard  什么是inflow  等等

你对它的看法

对开发者来说不仅仅是API的设计问题

而是一个API的生命周期

他们怎么可以从中学习呢

你应该怎么使它们一体化呢

并切你怎样能够在那上面做出一款成功的软件呢

所以当我们谈起开发经验的时候

我们需要彻彻底底的想想

以便能给开发者一个愉快的体验

也让你更容易将之加进你的程序中

把之前我们谈到的一致性作为一个例子

所以学习一个API的经验

会帮助开发者更容易的

开发下一个程序

Android平台是多种多样的

有非常多的版本

有太多的东西需要学习

才有可能成为最好的开发人员

那么我们正在做的Google Play services

对开发者有什么帮助吗

是的


与Android 2.3之后至今的所有版本

是有一点的不同的

已经发布的Gingerbread中可以看出

如果一个开发者

与Google Play services的API统一起来的话

我们可以保证

它可以在所以的这些设备上运行

帮助你成为拥有十亿活跃量的Android设备的

程序开发员

十亿

是的

能详细说明一下

让我正确理解你的意思吗

如果我使用Google服务编辑一个程序

并且使用Google Play services

然后在Gingerbread上运行

或者在KitKat上

再或者在Honeycomb或Lollipop上

我们都不需要做出一些调整吗

当然

另一方面  Google Play services

我们会提供自动更新

例如  如果你遵循统一的

使用我们提供的定位API

以后如果我们想出更好的方法

位置检测可以提供更高的精度

并且使用更节能的方法

你可以免费为你的程序得到那些

一旦开发者使用统一的话

你就不用担心了

并且你就可以得到更新的福利

有一个问题我要问一下

像Android一样我们一直在使用有趣的名字

例如Kit Kat FroYo Lollipop

那么Google Play services有没有奇怪的名字呢

我们准备把它叫cheeses


是的



是的

名字一定很难找吧

那我们现在到底叫什么cheeses呢

我们用了一种以N开头的cheeses

N 我想不到

哪种cheeses是以N开头的

好吧  其实我们稍稍作弊了

本来是Nacho Cheese

没有使用全称  我们公布为Nacho

太棒了

现在是N以后就是O

N后面是O  是的

你能告诉我们

你能告诉我们在下一个版本中叫什么cheese吗

下一个命名为Orla


我从没听说过Orla cheese

我准备到干酪店中买一些

那么在更换版本的时候

是否有一个新的切奶酪的聚会

有啊  有一个切奶酪的聚会

我们在那次切了奶酪

我们确实买了奶酪

我们聚在一起享受一个小型的庆祝

太酷了

我很期待Orla的样子

嗯哼

我们重新回到开发者这里

先不说cheeses了

我们生活在流行手机的世界中

并且开发者必须要比其他人

生活得更超前

他们在手机得势的世界中有着独特的挑战

这不同于网站开发或者桌面设计

更不同于云开发

那么你认为开发者到底面临什么挑战呢

我们有什么可以帮助他们的呢

当然  我认为制造手机应用

与建立一个网站是不同的挑战

例如  如果你仔细想想

你交给最终用户的代码

是运行在计算机上的

确实是一个细节问题

你不能控制吗

用户在某些地方时

可能会有网络很差的问题

电池也是人们关心的问题

因为用户将要使用它一整天

所以作为一个开发者

你需要从用户的角度考虑这些细微的差别

并且想办法让其达到最佳

考虑你怎么做可以让它运行快

可以在外面各种各样设备上正常运行

所以使用Google Play services

可以帮助你

我们想了很多优化移动设备的东西

就像离线链接一类的东西

并且作为开发者的话

我们不应该耗时考虑这些而是

应该专注于辨别你的程序并真正做出东西

来让你的应用程序更完美

可以让Google帮助你解决

契合移动设备的根本问题

太酷了

制造一个基本的设备

它只是你口袋里的一个微小的装置

却也有复杂的情况

使用Google Play services

可以很大程度上减轻这种复杂的情况

帮助开发者更好的编写程序

很显然

那你有些什么建议

可以让开发者成为

最好的当今移动开发者吗

使用Google Play services

是的  当然

他们可以立刻收获成效吗

当然

在我接触之前

我们只通过同一个SDK提供Google services

例如  统一Google Analytics

真的是一个好方法

去洞察用户在做什么以得到反馈

然后优化你的应用并建立更好的程序

再例如  使用位置访问服务

这会帮你找出最好的方式得到用户的位置

假如你要编写一个位置感知程序的话

所以你不用担心你是使用GPS

还是使用无线网网络  或是各种其他的东西

你只需要有一个定位的API

并且你可以将不同于你程序的东西

联系起来

然后按照各种类型优化你的电池

以让你不会过度使用它

是啊

太酷了

好的Francis  非常感谢你能来

与你一谈受益匪浅

我又了解了很多东西

希望屏幕前的观众也有所收获

这是我的荣幸

这非常有趣

哈哈

因此  观众朋友们  请记住这是

Coffee with a Googler的第二季

谢谢你的长期观看

如果你喜欢哪位谷歌职员

希望他来节目中一起谈谈

请联系我

给我们留言

你可以在YouTube上的Google Developers频道上

继续观看所有的Coffee with a Googler系列视频

谢谢



