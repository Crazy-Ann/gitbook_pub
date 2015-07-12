## Android Performance Patterns: Performance Cost of Memory Leaks

![video_screenshot](images/h7qHsk1nWKI.jpg)

** 视频发布时间**
 
> 2015年3月11日

** 视频介绍**

> Just because you’re working in a managed memory environment on Android, doesn’t mean your app is immune to memory leaks. And, as you start leaking more memory, the amount of memory available to your app continues to get smaller, which means that Garbage Collection events will be executed more often to try to free up space for normal program execution, which of course, chews through your performance.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 高冰 | TWL007 | ——| [ Youtube ]( https://www.youtube.com/watch?v=h7qHsk1nWKI )  |  [ Youtube ]( https://www.youtube.com/watch?v=hHUbjl5rsDs ) | 1503170424 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：


我们编写的程序运行在Android Runtime(ART)虚拟机里


最棒的感受就是


程序的内存使用会一直受到管理


你不用去担心对象在生成和被销毁时产生的


所有的额外的内存开销


但这还是要引起注意


即使在一种具有内存管理的编程语言中


程序仍旧可能会因为内存泄露而崩溃


我叫Colt McAnlis


在复杂的代码库的编写中  内存泄露问题是一个经常会被提及的话题


如果发现问题而不及时处理


可能会在app上引发讨厌的性能问题


你可能还会记得  ART中内存堆如何分段于空间中取决于


给程序分配内存的方式


和系统为了使垃圾回收机制更有效会


怎样合理组织这些堆内存


基于你的ART版本


当为新的对象分配内存空间时


通常都要考虑ART的这些特性来使其


适应其应当被放置的空间


这就是问题关键所在


每一份空间都有大小限制


当为对象分配内存空间时  我们会一直追踪整个程序所占的内存大小


当内存占用开始增长的时候


为了以后的内存空间分配  系统就会自动启动垃圾回收机制


去尝试释放掉一部分内存空间


一般情况下  垃圾回收的问题对于性能而言


都不太容易被察觉到


然而  垃圾回收被一遍一遍


一遍一遍地执行  就会使吞噬掉你程序的CPU的时间片


在垃圾回收上花的时间越多


在做其他事情上花的时间就会越少


比如在渲染程序或者播放音频时


现在 一个可以引起一连串垃圾回收动作的普遍问题


就是内存泄露


内存泄露是指垃圾收集器没有成功识别


程序已不再使用的对象


造成的后果是这些对象仍然占用着宝贵的内存


使那些内存无法分配给其他有用的对象


当你开始泄漏更多的內存时


内存堆中可分配的空间就会变得越来越小


也就意味着垃圾回收会比之前更频繁的执行


来尝试释放更多的空间给正常运行的程序


如果有很多垃圾没有被成功释放掉


程序就不会正常工作


找到并并修复内存泄露确实是件苦差事


有效的做法是  你要对你的代码了若指掌


确保你在代码库中的关键步骤的代码


按照正常的要求运行


判断内存泄露是否发生不管怎么样都需要经过一番仔细的检查


举个栗子  让我们假设你希望确保


当用户在app中


离开一个Activity时


与这个Activity有关的所有内存都会被正确清理


该怎么去做呢


首先  你要使用Heap  DDMS中自带的内存监测工


记录下当Activity最初打开时


占用内存的情况


第二步  创建一个可以让我们之前问题提到的Activity转换到的


空白并且拥有已知或


低内存占用的Activity


第三步  当这两个Activity发生转换时


强制执行一次垃圾回收


如果Activity的一切内存占用都被正确销毁


那么垃圾回首动作应该回收了所有的Activity内存分配


如果你在第二个的heap dump中看见一些可疑的东西


那些不应该出在那里的内存数据


聪明的做法是使用Allocation Tracker  内存分配跟踪器  继续分析


并深入研究内存的分配情况


利用这个工具  你可以追踪Activity内存分配


从它被载入直到被卸载和


你切换回那个空白Activity


Allocation Tracker会给出


一个已分配对象的列表


以及这些对象的创建顺序  以及他们在何位置被创建


这样一来你就可以去追踪那些不听话的内存


并弄明白他们为什么没有被释放


即使你在一个内存被管理环境中


为了让app保持优越的性能


你仍然要亲自做许多手工内存管理的工作


所以还请务必观看Android Performance Pattern Change


的其他内容


也别忘了在Google+上关注我们


里面有我们提出的一些其他的小窍门  小技巧


不要浮躁  一定要去测试你的代码  并时刻牢记确保程序性能的重要性






