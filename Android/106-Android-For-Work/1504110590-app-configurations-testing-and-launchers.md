## Android for Work - App Configurations, Testing and Launchers 

![video_screenshot](images/39NkpWkaH8M.jpg)  

** 视频发布时间**
 
> 2015年3月23日

** 视频介绍**

>  With Android for Work you can make your apps remotely configurable. In this episode we also cover how to test your app in a managed environment and have some tips for developer's of Homescreens/Launchers.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 葛伟 | 高冰 | ——| [ Youtube ]( https://www.youtube.com/watch?v=39NkpWkaH8M )  |  [ Youtube ]( https://www.youtube.com/watch?v=W2ytCaDZJ30 ) | 1504110590 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |


### 解说词中文版：

对于企业里的应用

由IT管理员统一配置应用数据

比让每个终端用户自己配置要好很多

比如在添加服务器URL  域名  白名单  黑名单  启用加密

甚至是新建用户名和密码等方面均是如此

我是Rich Hyndman

这是我Android for Work系列的第二集

本集视频会涉及到应用配置  应用测试  和启动器开发的内容

如果你还没有看过第一集  快戳这个链接

在Lollipop版本中  我们添加了可为应用单独进行配置的API

这样一来就可以由IT管理员远程配置应用

来决定一些功能是否可以开启

新建一个xml文件  在里面列出所有限制条件

IT管理员通过应用管理控制台

即可让这些限制生效

创建一个RestrictionsManager类的对象实例

或者访问get_application.xml文件

均可得到当前应用提供了哪些限制条件

如果在应用刚发布的时候这么做

你会发现管理员已经设置好了一些限制条件

但是这些限制条件可以在之后随时更改

所以你应该注册相关的广播接收器

如果哪天管理员更改了策略

你就能第一时间更新应用的配置

我说的这些你大可都不必记住

在Implementing App Restrictions里会有很详细的说明

和一些示例代码

打开developer.android.com/work来查看详细内容吧

对代码进行测试往往需要考虑很多条件

不管你是否对应用进行了额外的配置

在托管配置（managed profile）环境下测试应用

是非常好的实践

Android for Work提供了很多工具来帮助你完成测试

首先  你需要在你的设备或者模拟器中

添加一个托管配置文件

可通过BasicManageProfileSample这个Demo进行添加

在Android Studio欢迎页上

点击Import an Android Code Sample项可找到该项目

在这个Demo中可配置

哪些应用在该托管配置文件下可用

哪些intent可以在不同配置文件之间传递

接下来  当然是要安装你的应用

当在设备中添加了托管配置文件之后

安装的应用在不同配置文件下都可以打开

所以接下来你需要选择要以哪个文件的配置

运行这个应用

你需要在adb中传入user ID参数

首先得要找到每个配置文件的user ID  输入list users命令即可获得

在得到的结果中  每行的第一个数字就是user ID

如果你的应用要使用到相机等自带应用

可在配置文件中禁止掉这些权限  再去测试一下看看效果如何

最后  说一下启动器(Launcher)的开发

启动器可代替Android默认的主界面

为用户提供特别棒的定制桌面

如果一个应用同时有2个配置文件

要想让它能够跟别的应用不太一样  确实得在外观上稍稍做些修改

第一集中提到过

启动器为公司的应用图标均添加了一个工作标记

Android 5.0引入了LauncherApps类

调用LauncherApps类的getActivityList函数

packageName参数传入null

即可找到当前配置文件下所有可用的Activity

由于托管配置文件可随时添加和删除

你肯定想到了要注册配置文件添加和删除事件的回调函数

来让桌面显示的内容保持最新的状态

可调用这个2个方法

来得到带标记的图标和定制的文字

使启动器可以

正确显示这些应用

如果你的启动器支持窗口小部件(Widget)

在AppWidgetManager类中我们也添加了几个新的方法

来处理多配置文件的问题

今天就讲这么多

谢谢观看  咱们接着回去干活吧

