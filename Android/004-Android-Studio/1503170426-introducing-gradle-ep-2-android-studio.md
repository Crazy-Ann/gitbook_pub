
## Introducing Gradle (Ep 2, Android Studio)

![video_screenshot](images/cD7NPxuuXYY.jpg)

** 视频发布时间**
 
> 2015年3月13日

** 视频介绍**

> Android Studio comes with an entirely new and flexible Gradle-based build system. Using just gradle configuration files you will be able to create multiple build variants for a single project, manage library dependencies and always be sure that your application builds correctly across different environments, regardless if it’s an IDE, the command line or a continuous integration server.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| wang7x | 虞高 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=cD7NPxuuXYY )  |  [ Youtube ]( https://www.youtube.com/watch?v=iusMETwu4jw ) | 1503170426 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

WOJTEK KALICINSKI  你是否遇到过刚加入一个新团队

就必须尽快开始编码  却发现

设置各种工具和外部库

耽误了太多时间

对我来说当项目截止日期到来之前最后一件事

就是尽力让我的项目构建成功

这也是为什么Android Studio会提供一个易用

强大的基于Gradle的构建系统

它将从根本上提高你的工作效率

Gradle崇尚约定优于配置的规则

它提供实用的（sensible）默认设置帮你上手

同时考虑到了其他更高级的功能  例如更好的

库管理机制  内置多APK支持等等

让我来展示一些例子

你的构建设置和所有项目的依赖

都用直观的声明语句保存在Gradle构建文件中

这些文件是你项目情况的唯一来源

这意味着你在这里所做的任何改变

都将自动的反映在IDE中

例如  类似代码自动补全这样的功能

会始终与你的项目配置保持一致

更吸引人的是  这些构建文件

支持在命令行运行Gradle时和

在你的持续集成服务器上使用 

以确保在任何环境下的一致性和可复用性

如果你已经使用了很长时间的Android Eclipse开发工具后 

去学习一个新的构建系统是一项艰巨的任务

这是为什么从Eclipse导入一个项目时

Android Studio会自动为你创建Gradle配置文件 

甚至能识别通常被使用的库

并将它们加入依赖中

你的应用程序的一些基本设置  例如应用程序ID

支持的最低版本和目标版本SDK以及版本信息

现在都包含在构建文件的默认配置区

你能在依赖项区域找到

你项目依赖的所有本地和远程库

当导入一个项目Android Studio

不能正确识别依赖项时

或者你想要增加一个新库时

你可以通过Maven搜索对话框轻松地找到正确的包名和版本号

并设置在依赖项区域

如果你仍然感到迷惑  只是想要

快速上手  你可以在Gradle.please网站上找到

类似F-Compact或

其他实用的库的例子

创建或使用第三方库的另一个问题是

没有有效的办法

跟代码一起发布Android的特定资源

你要么不得不四处移动目录

或者只能使用一个JAR包  这个只能包含java类的文件类型

有了Gradle  我们引入

Android归档格式  缩写AAR

使你能发布或附加

一个包含源码  图片

甚至项目manifest的一体库到你的项目中

Android Studio带来的不仅仅是更棒的

库管理机制

你是否曾需要构建出你应用程序的多个版本

同时又处理代码复用或其他类似问题

借助Gradle的灵活性  你可以给同一个项目

创建不同的版本

默认有debug版和release版两种编译类型

加上你设置的产品定制版本

这些集合在一起  我们称之为多样性构建

构建类型和产品定制是一种

非常强大并且可自定义的概念

例如  你可以为每一种构建类型

分别定义签名设置  或你想

在Play商店上传一个免费和一个收费版本应用时

你能够控制两个定制版本的应用程序ID

即我们说的包名

简单至极

此外  每一个类型  定制版本和变种版本

都能够包含它特有的一小块代码和资源

这些代码和资源会与主代码基础合并在一起

甚至还可以为特定的定制版本指定附加的权限

组件或者重写manifest设置

而不影响其他的定制版本

你能够结合这种机制和多APK包支持特性

在Play商店中创建并发布基于不同设备的特有的APK

以适配不同的屏幕分辨率  CPU类型和API等级

这样做一个重要的好处是能给你带来更好的开发体验

并且你的用户需要下载的应用大小也更小了

当使用变种构建版本时  Android Studio

只会在项目概览界面中显示当前版本

对应的文件

使用构建变种版本面板  

可以改变当前编辑的应用版本

你也可以在Gradle侧边栏中检出

每一个变种版本自动生成的构建任务

可以使用这个功能模块

如果想要为你的应用构建所有可能的设置

如你所见  有了Android Studio  我们终于拥有一个现代  强大

能够使你从管理项目的痛苦中解脱出来的构建系统

在这个视频中  我们初步了解了Gradle能够做到什么

如果你有任何其他的疑问

请加入我们的Google+社区

敬请期待后续的Android Studio视频




