## Layout Editor (Ep 3, Android Studio)

![video_screenshot](images/JLLnhwtDoHw.jpg)

** 视频发布时间**
 
> 2015年3月25日

** 视频介绍**

> The difference between a text editor and an IDE is all in the tools that support your development flow. Android Studio includes a rich, visual layout editor that helps developers create better user interfaces. It eliminates the need to deploy the APK on a real device with each change, making iterations faster and helping eliminate common errors earlier in the development process. In this video you will learn a few layout editing tips that every developer should know.Watch all Android Studio videos at: https://goo.gl/SUqTzcSubscribe to the Google Developers channel at: https://goo.gl/mQyv5L

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 葛佳恒 | wang7x | —— | [ Youtube ]( https://www.youtube.com/watch?v=JLLnhwtDoHw)  |  [ Youtube ]( https://www.youtube.com/watch?v=eWXs3G5BwA4 ) | 1503290479 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

我热爱写代码

但是如果你和我一样

那么为你的应用构建最复杂的逻辑

都比创造一个优秀的用户界面容易

设计是随着时间变化的

在设备上测试布局的每一个变化会异常枯燥

进入布局编辑器  它是Android Studio内置的一个工具

可以让你实时地编辑和预览布局

不需要重新编译后

再把APK安装到真实设备或者模拟器上

布局编辑器会在你打开一个XML布局文件的时候

自动运行

设计视图可以让你通过从面板向编辑区拖拽组件的方式

来便捷地添加和摆布这些组件

可视化的辅助线帮助你按照相对位置放置View

考虑到所处父节点的类型

以及要求的布局参数

你可以在Inspector中编辑其它的View属性

或者在组件树状面板中改变View在布局层次中的位置

在你已经设置好了一个View之后

又想改变它的类型时可以使用一个便捷的技巧

只需要右击View  然后从变形（Morphing）菜单中选择

你想要的组件就可以了

需要注意的是  有些不合理的

修改是不允许的

比如说  你不能将一个线性布局更改为

一个TextView

当你发现布局层次中的某些部分

可以在其它布局复用时

有一个抽取布局的重构选项可以帮助你

当你使用它时  你选择的子布局

会被移到一个单独的资源文件

并且被包含进当前的布局

当你打开新的文件进行编辑的时候

你可以看到它依然是嵌入在

之前的布局层次中进行预览的

这是因为Android Studio在重构的时候

向XML文件中加入了一个特殊的标记

让我们来看一下  点击Text标签

切换到原始XML文件的编辑状态

注意到不同于可视化编辑器

现在当你编辑代码的时候

会有一个实时更新的预览窗口

如果你总是更喜欢查看代码  而不是默认的设计视图

只需要打开这里的偏好XML编辑器选项

我刚才提到的渲染的标记

实际上包含两部分

首先  在XML根节点上有一个新的tools的命名空间

其次是一组特别的注解

它们不会在运行时生效只会被Android Studio处理

这里可以看到showIn属性

它会把你正在编辑的布局文件

添加到另外一个布局中的include标签的位置进行渲染

这功能很有用  但是还有另外一个

大大提升效率的技巧

我真希望有人早点告诉我这个技巧

实际上你可以通过加上tools命名空间的前缀

来覆写View的大部分属性

听起来很简单  但我们还是看一下它是如何工作的

以前编写布局时只能有空白的TextView

因为没有适配器来提供数据  比如在一个ListView中

使用tools命名空间添加测试的文字

这样就可以立即查看布局的样子了

如果布局的一部分被设置为Gone或者Invisible

只能根据运行时的条件进行显示  这种情况怎么办？

只需要在设计时覆写tools命名空间的可见性

如你所见  布局编辑器是非常棒的工具

而且你可以在Android Studio中使用它

如果你想学习更多或者你有其它的布局编辑技巧

在Google+的Android Studio社区里和我们分享吧

另外一定要看看Android Studio Devbytes系列

的相关视频




