## Google Root Access: What we learned building plug-ins for Android, with startup Magnet

![video_screenshot](images/lboyR-A1woU.jpg)

** 视频发布时间**
 
> 2015年3月2日

** 视频介绍**

> Magnet has been successful building Android plug-ins to reach developers and drive adoption of Magnet's platform. Pascal Jaillon shares what they learned, in conversation with Martin Omander.For startup specific video content, subscribe to the Startup Launch channel here: http://goo.gl/vf6Ngg

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 虎子 | eternity | -- | [ Youtube ]( https://www.youtube.com/watch?v=5gArR3JACBI )  |  [ Youtube ]( https://www.youtube.com/watch?v=52yzGPXG3lI ) | 1503230453 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

 MARTIN OMANDER  今天，我们的嘉宾是Pascal Jaillon  

他领导了在创业磁的开发者项目  

Pascal  欢迎来到现场  

PASCAL JAILLON  谢谢  

MARTIN OMANDER  那么  Pascal  你能

告诉我们一些关于开办创业磁项目的事情吗  

PASCAL JAILLON  好的  磁提供了

一系列为开发者准备的产品套装

用来开发很棒的移动应用  那些应用

充分发挥了这些能装在我们口袋中的

微型计算机的计算能力  

MARTIN OMANDER  嗯  不错  

那么你在工作中使用哪种谷歌开发者工具呢  

PASCAL JAILLON  显然  我们开发安卓应用  

而且我们使用谷歌能够提供的所有开发工具  

从众所周知的Mini-SDKs  老版本的

IDE  到  生成器  所有的工具我们都使用  

现如今  开发者们从不尝试去

讨论任何关于用户们

在哪种平台上使用这些移动应用  

所以  在Magnet  我们确保我们能够开发出

适用于自然界中所有设备的应用  

MARTIN OMANDER  怪不得我还没有

从你这里听到过  平台  这个词

但是我猜这个词会出现的  

我也是一个开发者  而且我认为很多的开发者

当听到  平台  这个词的时候总是有些紧张  

因为这意味着必须重写新的基础代码

你不会知道这个新平台的优势和弱点


说真的  对于一个开发者来说

切换到某种完全陌生的东西之上  这很让人恐惧  

你怎么解答这些开发者们关心的问题呢

PASCAL JAILLON：恩  听我说

人们  开发者们 一开始总想尝试一下  对吗

所以  你构建的平台越大

你实际上就越是在把这个平台碎片化  变成了一些组件，

那些组件能够单独测试  彼此独立

而这正式我们在Magnet所做的 

我们正在定位不同的精细之处

这些精细之处为开发者所拥有  从连接  到实时

通讯  到远程控制

而所有的这些点在不同的产品上都得到了而定位

MARTIN OMANDER：啊  所以开发者可以进行尝试

而且进行浅度的使用  而不用去整个地理解

这个平台 

PASCAL JAILLON：对的

而且让开发者能够进行尝试，

这一点很重要  典型来说  我们的新的信息传达

解决方案  我们正在进行一个云端的版本 

所以开发者们可以只是进行试用  并且

根据这个是否有效来决定是他们是否去在他们的自己的产品上使用这个平台 

MARTIN OMANDER：构建良好的开发体验比较困难

我是说  我们尝试着在谷歌这里做这件事 

而你们也在尝试

我想  这必然造成大量的重复

在你们准备好装载一些东西的时候  

PASCAL JAILLON;肯定的

而且  对我们来说  理解开发者

是如何工作的  他们如何开发移动应用，这一点非常重要

所以我们需要确切地了解他们工作的

方式  了解他们怎样构建你的那些用来解决需求的产品  

所以  关注需求关键需求很重要

而且  在rest2mobile  也就是第一个用来定位连接的产品的情况下

我们发现

要想维持开发者的流量

最好是真正地去为各种IDE构建插件程序 

而不是采用通过浏览器来

下载整个SDK的这种潜在的竞争性解决方案

我们想在他们的IDE里面完成任务

将开发者维系在他们的IDE中

这将使他们在那里码代码  并富有生产力

MARTIN OMANDER：你提到了IDE

在安卓平台上，开发者们使用各种IDE

你是怎么处理这种状况的

PASCAL JAILLON：嗯，所以我们希望能确保

他们在不同的IDE上有着相同的用户体验  不管是在iOS  还是在Xcode上

所以我们做了比我们预想的多得多的大量工作

但是我们选择的IDE 是Android Studio

因为我认为这是谷歌官方的

作为额外好处  我们我们使其能和IntelliJ一起工作

因为这是一个不可见的代码基础平台

但是我们也构建了一个自动化的命令行工具

为了那些不在IDE里工作的开发者们

而我们也为Xcode开发了另一个插件

这增加了我们的工作量  不过还好

MARTIN OMANDER：也为Eclipse开发了一个吧

PASCAL JAILLON：你可以使用Eclipse 

但是我们并没有为Eclipse开发一个全功能的插件  

但是我们的命令行工具能帮助那些

在Eclipse下工作的开发者们在他们的移动应用里生成代码

MARTIN OMANDER：我明白了

那么  在哪找到大多数的开发者们的兴趣所在呢

人们是否正在转Android Studio 

抑或是还在Eclipse上  

PASCAL JAILLON：我们所见到的是正在向Android Studio过渡

这是一个很棒的IDE 

它运行良好  

用户体验也很棒  

他们收到了大量的反馈 

和大把的用IntelliJ IDEA完成的工作

所以那绝对是一个绝好的平台

用来进行安卓应用的开发

MARTIN OMANDER：当我从我们的[INAUDIBLE]中

下载了这个插件  并在我的IDE中安装了它  会怎么样呢

它能怎样帮助我  作为一个开发者

PASCAL JAILLON：通过这第一个产品  也就是

rest2mobile  我们希望能够帮助开发者们

构建他们的连接性的APP  去把他们的移动应用

连接到REST API和REST services  

这有点复杂  

必须要处理到服务器端的远程连接

还要处理JSON数据库的荷载

MARTIN OMANDER：在互联网时代  任何互联网产物——

都会过时 

PASCAL JAILLON：的确是这样

我正在为实现一些离线功能和工作

所以我们想通过一个插件提供

这种独立的功能

所以我们用代码生成器

我也知道 有时  代码生成器名声不好。

MARTIN OMANDER：是啊  听到代码生成器，

吓得我都坐到地上去了呢（我表示严重怀疑！）

那会生成我无法修改的代码的  

那可是种神奇的代码  我要是改动了一下  就会崩溃滴

我无法很容易的重新构建它 

PASCAL JAILLON：当然了  我们希望

能确保这不会让开发者来操心

所以我们生成了我们能生成的最好代码

确保这些代码能

在你的移动应用里

像你自己写的代码一样好（前提是你的代码是自己写的~）

但是我们会从你手里接过担子

我们为你创造这些代码

确保它 容易进行单元化测试

它[?和 单元化的测试同时?]

她很容易重新构建  对那些不止反编译一次的应用来说


这存在一个完整地生态圈 

所以  变得能够重新构建  能够变化

是非常重要的  我们通过我们的插件来实现这一点  

MARTIN OMANDER：我明白了

所以当为安卓生态系统进行构建的时候

你觉得你从中学到了什么

而你又想

和其他的和你处在相似位置的创业者分享哪些经验呢 

PASCAL JAILLON：确切地说  安卓

比起苹果来说  更加开放。

所以这很棒  因为这意味着有更多的文档。


这让我们构建插件的工作容易了一点  

同时  也存在很多如你先前所说的大量的IDE  

所以我们必须在不同的平台  不同的IDE上解决问题  

为不同的代码基础平台进行构建

不过挡在Xcode上构建插件的时候 

这种情况并没有发生  

但是同时  我们所拥有的文档很少  

所以我们不得不去查看————比如Github上的项目

并且和用其他的项目来理解如何去

为不同平台的开发者提供相同的体验 

MARTIN OMANDER：不错 

谢谢你能来  Pascal 

更感谢你同我们和我们的观众分享你的经验  

PASCAL JAILLON：谢谢你邀请我  

MARTIN OMANDER：我们希望你能找到一些

能在你的创业中使用的经验  

你的意见很重要 

请在下面留下你的评论吧  

我们会认真阅读的

去了解谷歌能怎样帮助你的创业 

去看看developers.google.com/startups.

如果你想成为节目上的嘉宾 

到bit.ly/applyrootaccess看看吧

暂时就这样

下次再见  