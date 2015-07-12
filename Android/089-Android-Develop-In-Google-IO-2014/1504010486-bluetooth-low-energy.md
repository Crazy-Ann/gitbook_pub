## Bluetooth Low Energy 

![video_screenshot](images/2fZThdNbHcQ.jpg) 

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> Bluetooth Low Energy is an incredibly exciting technology with the promise of unlocking a myriad of use cases. This session will focus on new Bluetooth Low Energy features, including improved scanning and newly added support for peripheral mode, in Android.

** 视频推介语 **

>  暂无，待补充。

### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| Wallace4ever  | 點墨 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=2fZThdNbHcQ ) | [ Youtube ](https://www.youtube.com/watch?v=GJ-Tab8Tqc8) | 1504010486 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator ) |


### 解说词中文版：

MATT GAUNT: 嗨

我是Matt Gaunt  是Google的开发技术推广工程师

在本次的视频中  我们将会看到一个不断变动的猴子

以及用有趣的机器人声音说话

而且我甚至可以来一个夏威夷旅行

这都归功于最新的Android WebView

当我们发布Android KitKat以后

WebView控件就从WebKit内核转变为了Chromium内核

预装为Chrome 版本M30

这个版本的优势是支持了开发人员工具

在KitKat的MR2版本中  我们把WebView的版本从M30升级到了M33

这意味着除了一般的安全更新和Bug修复

你还会得到一个全新版本的Chrome

WebView团队还努力提升了Canvas类的性能

并添加了对截屏和开发人员工具的支持

在最新的开发者预览版的Android L系统上

我们把WebView升级到了M36

并且启用了许多附加的Web平台特性

如果你还没来得及尝试使用开发人员工具来调试你的WebView控件

你只需要把这行代码添加到你的App中

设置setWebContentsDebuggingEnabled为true

你就能开启开发人员工具

当然我承认这个变量名字有些拗口

你可以只为调试版的App开启此功能也可以只为发行版的开启

这都取决于你自己

一旦你启用了这个功能

接着把你的手机用USB线接上电脑

打开你电脑上的Chrome浏览器  并跳转至chrome://inspect

你在这里能看到你的App中每一个WebView的详细信息

点击inspect将会启动开发人员工具

还有一点值得提醒的是

你需要一个版本与内置的Chrome相同

或者更新的桌面版Chrome

所以对于Android L的开发者预览版

你就必须需要使用Chrome Beta版本或者Chrome Canary版本

当DevTools开启的之后

我们就可以查看Webview中的DOM和CSS

这里你可以修改它们

并即时观察对你的App产生的影响

JavaScript控制台对观察console.log中的信息非常有用

就像手动在WebView中

执行JavaScript脚本一样棒

另外  一个非常有用的技巧是

如果你的WebView添加有JavaScript接口

你就能直接

在JavaScript脚本和原生应用中交互

你可以从开发人员工具控制台

直接调用原生方法  这可以让调试这些

桥接逻辑的时候更容易一些

Network页可以让你观察

页面上正在发生的网络请求

这对于需要从远端服务器加载页面

的App非常有用  只需要一个普通的URL

这对那些需要从APK文件中加载静态网页的App也非常有用

因为它们使用XHR调用

你可以看到这些控件的请求和响应

它们都会显示在Network页上

这要比在页面中写记录代码要容易些

这是时间轴

如果你注意到你的Web App有任何的延迟

这就是你需要仔细检查的地方

看看Chrome在每一帧上花费的时间

通常情况下你需要注意耗时任务

和重复执行的任务

看看有没有别的方法处理这个方法

我想提到的最后一件事是开发人员工具里的截屏功能

截屏功能在KitKat MR2及以上系统版本中被启用

它让你能够直接从开发人员工具里

和Web App进行交互

这意味着你不需要从电脑

转换到设备

你可以在电脑上做一切事情

这一点的好处是

假如你有一个WebView  现在为不可见状态

我们可以一会儿用动画显示它

你可以用截屏功能

查看WebView是如何渲染的

即使它不可见

我提到过WebView团队

提升了Canvas类的性能

这里我们有一些来自于Vellamo Benchmark套件的数据

你会发现这些任务的性能提升了200%到350%

我们再看看一些我在一开头

就提到的新特性

从我说过的不断变动的猴子开始吧

在Android L的开发者预览版中  我们支持了WebGL

这是来自Paul Lewis的一个实例

坦率的说  我非常喜欢这个猴子

下一个是Web audio控件

Web audio API是Web游戏的重要组成部分

它让你可以操作声音

创造和弦  使用麦克风输入的语音

这就是为什么我现在有了类似机器人的声音

最后一个特性是启用了WebRTC功能

你现在可以使用数据通道来

分享或获取用户媒体来访问摄像头

这就是意味着我可以做这样的事情

Sam你好

SAM: 你好Matt

最近怎么样

你在夏威夷

MATT GAUNT: 就像这样

我们提到了开发人员工具，看到了基于WebGL的不断变化的猴子

我可以用机器人的声音说话

还用绿幕去了一趟夏威夷

要获得基于Chrome的WebView的更多信息

请访问这个链接

祝你好运

