## Game On! - Frequency Scaling

![video_screenshot](images/AZ97b2nT-Vo.jpg)

** 视频发布时间 **
 
> 2014年9月10日

** 视频介绍**

> In the world of mobile computing, battery consumption and thermal regulation are everywhere. Android devices can scale back the amount of power sent to your CPU, reducing it's performance any time battery, or heat becomes an issue. For game devs out there, this can have a dramatic impact on your frame-rate, if you don't know what you're looking for.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| Alice | 隆斯朝 | —— | [ Youtube ]( https://www.youtube.com/watch?v=AZ97b2nT-Vo )  |  [ Youtube ]( https://www.youtube.com/watch?v=AZ97b2nT-Vo ) | 1505050797 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

当代的智能手机不得不在

性能  热输出和电池消耗

之间做出权衡

通常情况下用户在购买手机时

最后才会考虑这些问题  我的名字是 Colt McAnlis

你有所不知  对于游戏设备来说  这些物理属性

会带来一些非常奇怪的性能问题

你知道所有的当代的移动 CPU

都具有变频功能

也就是为了省电

硬件会根据多种因素来决定

是否可以降低供给 CPU 的电压

降低能量供给能够帮助

减少电池消耗和热输出

但是带来的负面影响就是减慢 CPU 的速度

目前  有很多种因素能够导致降压发生

你需要知道其中的两个

第一种频率调节

与 CPU 的负载量有关

如果你的 CPU 正在稳定的工作

然后突然  只有低计算量的帧持续的送给 CPU

这时 CPU 中控制频率的控制器

就可以降低供给频率

降低用于计算的电量

从而省电

当然  后续的帧

就会需要更长的处理时间  因为 CPU 的电压被降低了

那就意味着你将会看到你的帧处理时间增加了

这就会带来一个问题  当你的 CPU 的负载恢复到

正常状态时

因为频率被降低了

你的 CPU 的处理速度比较慢

可能会导致巨大的性能峰值

这个性能问题会持续到

CPU 控制器决定提升频率

回到你最初的状态为止

好消息是这种调节

是完全受你控制的

你可以在事情变得糟糕之前解决它

通过监控你的 CPU 帧 你可以很容易的

看出什么时候 CPU 持续工作在负载较低的状态

你可以在下几帧增加一些负载

以保证 CPU 工作量足够

持续工作在正确的帧频率上

这样可以保证你的 CPU 不会降频

从而减少你的帧处理时间的峰值的出现

顺便一说  循环

或者是特别好的解决方案可以减少帧处理时间

或者你可以做一些更高端的

例如200个僵尸实体的路径选择

但是那就是另一个话题了

幸好你的 Android 设备会汇报在你的设备上

实际发生的频率降低的数量

你可以决定这是否是一个真的问题

想得到这些信息

你只需要从奇怪晦涩的系统路径中读取一些文件

然后你可以得到你是否需要

人工干预

第二种调节

更加难办一点

因为所有事情都是

由设备的热属性决定的

在移动计算领域  其中一个主导趋势

就与热量分布有关

通常对于台式机 CPU 来说

它们都有讨厌的大大的散热风扇附着在上面

从而控制热量  保证你的电脑不会被烤融化

然而  移动设备不具有

足够的空间放这么大的风扇

必须要找其他的途径散热

更甚的是  每个制造商

喜欢采用不同的热属性

并实现在他们的设计中

例如  有些 Android 设备

用于处理长时间的游戏

而有些是希望处理正常水平的应用

所以可能不会提供足够的空气流通或者散热空间

从而便于有效的控制热量

正因如此  一旦散热成为问题

控制器就会调节 CPU  从而降低

CPU 硬件生成的热量

最终

由于形状参数或者运行时间等因素

你的 CPU 可能会过热  然后被调节

并一直处于降频状态  直到设备的热属性回到

正常操作值为止

一旦处于这种状态  你的 CPU 帧处理时间就会变慢

一般来说 没有好的方法

处理这种调节

因为它跟你的代码关联很小

主要取决于设备的热属性

除非你的代码做了一些非常疯狂的事

例如在手机上进行蛋白质折叠计算

那么这就是你的错了

积极主动的开发者会搜集

他们游戏运行的设备的性能参数

并针对这些设备采用降低运算的复杂度  特性

和运算质量等相应的方法

但是即使如此  避免热问题

还是有很多的工作要做的

当然避免各种热调节

的第一步就是

竭尽全力优化游戏的性能

以保证你不会在客户的设备上浪费电量

帧时间处于正常状态  热量输出正常

所以  像往常一样保持冷静

写代码

记住性能问题






