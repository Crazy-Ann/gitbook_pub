## Route 85 - Quick Tip: Don't Default that Switch!

![video_screenshot](images/SpMIYtl_A98.jpg)

** 视频发布时间**
 
> 2015年1月16日

** 视频介绍**

> The Google Developers show for iOS developers- In the first of our series of Quick Tips, we explain why Objective-C (and Swift) developers might not always want to add a default case to their switch statement when working with enums. Trust us, it's more interesting than it sounds.Want more Route 85 videos? Find them here: http://www.youtube.com/watch?v=cvyk5i...Subscribe to the Google Developers channel here: http://goo.gl/mQyv5L

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 鲁登科 | 程路 | —— | [ Youtube ]( https://www.youtube.com/watch?v=SpMIYtl_A98 )  |  [ Youtube ]( https://www.youtube.com/watch?v=SpMIYtl_A98 ) | 1501190371 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

欢迎回到Route 85

这是我们精心为iOS开发者准备的节目

非常感谢你的关注

很高兴与你同行

在此次节目中  我将会为你讲述

来自我们Google Maps团队的Tom告诉我的

一个开发小技巧

本次周更我们就讲这个小技巧了

我不认为会频繁做这样类型的视频

所以我称之为 Quick Tip

感谢Tom为我们带来这些

举个栗子  我们要写一个扑克牌游戏

来玩标准扑克牌

在PlayingCard.h头文件里

我准备用枚举来定义四个花色

开整

现在看起来还没什么问题对吧

随后我们会把它声明成为属性

现在我们要以这些为基础

为四个花色写一些方法

在扑克牌游戏中  我们计算得分的时候

不同的花色会有不同的分数

因此我们要写一些代码

将花色转换为分数

很明显我们要使用switch语句来解决了

我们将它加在这儿

我们要分别为黑桃  红桃  方块  梅花设置不同的处理

我们还要在最后添加default语句

呵呵哒  default语句里写点啥呢

我的意思是  这里根本就不会

执行到  对吧

我们已经把所有花色的情况都设定好了

如果真的执行到这里的话  就是业务逻辑有问题了

我们应该让我们的代码更严谨  对吧

所以我们在这里抛出一个异常

然后注释写上 //永远不会发生

我们在这里  抛出一个异常

因为我们的游戏真的处在一个非正常状态下

所有的软件攻城狮们都能明白

这种图样图森破的注释(永远不会发生)

很大程度上就是在盼着

未来的某天真的发生  让你措手不及

我们回到扑克牌游戏中

设计师大大突然决定

我们需要添加大小王

大小王牌有它们的得分情况

一只勇敢的攻城狮被指派处理这个任务

他们也认为我们只需在枚举类型中添加大小王即可

但是  随着我们代码量的增多

我们的工程师可能忽略了更新getPointMultiplier()这个方法

我们之后所有的代码  也可能使用到那个枚举类型

所以这个方法没有更新

然后发生了什么

就是这样

我们触发了default语句

代码报错啦

因此我整个人都不好了

如果你很幸运

在编译测试的时候就可以找出这个错误

如果你的幸运微微不足的话

会在上传苹果商店审核的时候  被Apple找出来

最点儿背的是

这个bug现在么有人发现

直到你的用户使用它的时候  说不定在你正

在被记者采访光荣事迹  突然  王炸  BOOM  你的程序崩了

呵呵哒

请允许我做一个悲伤的表情

那么你要怎么做才好呢

答案也许会

会出乎你的意料

我准备从switch循环的末尾

移走default语句

这看起来脑子进水了  是不是

是不是脑残了呢

我的第一反应是我要把它放回去

但是先来看看我移除了default语句之后发生了什么

还木有运行  Xcode就提醒我说

switch循环现在是不完整滴

你要修复它啊  好孩子

它很智能  知道我没有把所有的选项都列举出来

它给了我一个很有用的警告

事实上  在这种情况下

我不仅得到了警告

而且发现了一个错误

这个方法没有返回值  程序连编译都不能通过

顺便说一句  如果你正在使用AppCode

点击Alt-Enter是会自动弹出提醒你

switch语句不完整  它会自动帮你

补全缺失的代码

太赞了  元芳你说呢

如果你进行Swiftees测试的话  条件会更苛刻

它会将警告升级为错误

它不会让你编写任何

不完整的switch语句

它会建议你添加default代码块儿

眼见为实  那有可能不是最好的提议

很显然你可能不会处理所有的状态(这里缺了case 4)

如果你要写一个基于整型的switch循环语句

或者是文本形式

Xcode无法知道你是否包含了所有

事实上  在这种情况下

Xcode会直接提醒你  需要添加default语句来加以修正

但是如果你的switch语句是基于枚举类型

并且你认为default的情况不会出现

那么就可以把default给删了  让Xcode帮你处理这些错误

而不是让用户来吐槽

这就是今天的节目

再次感谢的Google Maps iOS团队的Tom

为我们带来的这些小技巧

那么各位亲们感觉如何

你对今天的 Quick Tip

有没有一些好的建议呢

把它发给我

你可以通过这个地址给我发邮件

建议一旦被采纳  我将会送出一些小礼物的说

我不确定会送什么礼物给大家

比如T恤衫或者钥匙扣  也有可能是iPhone6或其...

哈哈哈

好的吧

晓得了

不送iPhone6哈哈哈

我们有T恤  那就送它吧

再次感谢您的收看

你继续写代码

我们在下一集Route 85中再见

卖个萌  拜了个拜




