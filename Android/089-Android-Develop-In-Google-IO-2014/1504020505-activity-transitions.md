## Activity Transitions 

![video_screenshot](images/RhiPJByIMrM.jpg)  

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

>  The L Developer Preview adds a new way to improve navigation between Activities and Applications. With the Activity Transitions API, developers can easily add animations between Activities, including enter and exit animations as well as animations on shared elements. Take a look at how easy it is to add transitions between Activities.

** 视频推介语 **

>  暂无，待补充。

### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| TWL007  | 韩晓健 | 暂无 | [ Youtube ]( https://www.youtube.com/watch?v=RhiPJByIMrM ) | [ Youtube ](https://www.youtube.com/watch?v=HTTT5XRRy2E) | 1504020505 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator ) |

### 解说词中文版：

嗨  大家好

我是来自Android UI开发工具团队的George Mount

我来介绍一下我们在Android L开发者预览中推出的

全新的Activity Transitions API

在我们开始说Activity Transitions之前

让我们稍微说一下转换

转换协助你的程序给用一个连续的反馈

在这个程序中  在左右两边我放置了按钮

当我们点击按钮的时候 会发生一些变化

但是并不够明了

现在使用在KitKat中开放的Transitions API

仅仅需要几行代码

用户就会清楚地明白

按钮在不同列之间移动

Transitions API同布局工作时表现非常出色

但是我门可以让它在不同的activity间工作么

默认的Activity Transition有一个缩放和淡入淡出效果

我在我的手机上演示这个效果

这样就显而易见了

我们可以自定义Activity Transition的效果  比如  淡入淡出效果

我们也可以使用缩放  滑动 或者旋转效果

但是它们与全屏冲突

并且不能给与用户我们真正想要的连续性的效果

对于新的Activity Transitions API

如果我们想要连续性效果

我们必须亲自去创建它

这里我们有一个Activity A

这个Activity带有一个我们想要用来转换到

新Activity的黄色视图

现在 如果用以前的方式来实现

我们要做的第一件事情就是必须获得这个共享元素的

大小以及位置

下一步 我们启动activity  覆盖目标中的位置

我们的新Activity 命名为Activity B

必须创建一个透明背景的半透明窗口

它当然也会阻止默认的缩放和淡入淡出效果

之后共享的元素视图会被

测量大小然后放置在处于目标中的位置

之后背景淡入  然后共享元素可以

变换到它最终的位置上

之后我们其他的UI元素可以出现

哇哦

真的是好费事

让我们来看看新的Activity Transitions API是如何工作的

这里我有个联系组 里面全是我英俊帅气的同事

当我点击他们的头像的时候 

它会使用另外一个activity来显示详细的联系人信息

我想在两个activity间共享头像

来描绘用户头像

因为我可以拥有任意数目的共享元素

我需要在不同的activity间给我联系人中一一命名

我只有一个

我命名它为Contact Image

为了告诉框架哪个视图会成为共享元素

我也给图片命名了

我以同样的方式给它命名

这样我就不需要任何代码来将联系人名字绑定到

共享元素上

我也希望共享元素能返回到grid中

所以我也命名了那个元素

之后我只要将它与activity选项软件包一同载入

让我们看看它看起来是什么样

看起来不错  并且我们不需要做任何复杂的工作

当方向改变  共享元素会从

调用的activity中获取最终的位置

然后恢复到正确的位置

真的很神奇

我的activity相比共享元素执行了一次

细微的淡入效果

我想要一些更引人注目的东西

让我们使用漂亮的滑动效果

来设置进入转换  这样其他的视图

就会从底部滑入

之前  调用activity并没有任何效果

我喜欢环绕在共享元素周围的视图

使用扩散效果来离开

让我们看看这个看起来是什么样子

当进入activity中的视图向上滑动的时候

调用activity中的视图

从画面中推了出来

我可以通过让进入activity在

它划入前等待调用activity结束来

让转换变得更加引人注目

现在你知道在你的activity间

加入连续性效果是有多么容易了

我知道你们准备在你的

程序中加入活动转换了

确保你会查看更多的DevBytes

以及I/O其他的视频

感谢观看
