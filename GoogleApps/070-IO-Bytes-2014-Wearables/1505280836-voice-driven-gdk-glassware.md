##  Voice Driven GDK Glassware

![video_screenshot](images/vGotlqDeUGk.jpg)

** 视频发布时间**
 
> 2014年6月21日

** 视频介绍**

> From voice command menus to collecting open ended speech input, this codelab will teach you about all of the available voice APIs to create a compelling Glass application.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 高冰 | 虞高 | -- | [ Youtube ]( https://www.youtube.com/watch?v=vGotlqDeUGk )  |  [ Youtube ]( https://www.youtube.com/watch?v=Ee_8gdLI268 ) | 1505280836 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

大家好  我是Google眼镜团队的Amin

今天我将向你展示如何创建

一款带有声控功能的Glassware（Google眼镜的应用）

我会向你展示可利用的API  并教你如何使用它们

首先  播放一段用Google眼镜

操控Google地图的示范视频

OK Glass  告诉我怎么去旧金山

OK Glass  向我展示行车路线

该Glassware使用到了两个语音相关的API

第一个是voice trigger

它将get directions to指令识别成

让Google地图进行导航

第二个是contextual voice menu

有了它  就可在说完OK Glass之后得到一个可定制的指令菜单

具体看一下这两个API

要在Google眼镜的主页启动你的Glassware

首先得要找到对应的voice trigger xml文件

这个文件会详细说明要用哪一条

指令来启动你的Glassware

会声明出你的activity都需要获取哪些权限

你的Glassware是否需要语音识别功能

在这里  navigation trigger.xml要指定GET_DIRECTIONS_TO作为启动指令

需要获取网络权限

并且当打开应用之后还需要语音识别功能

接下来  在AndroidManifest.xml中的<activity>标签里

与voice trigger进行关联

显示的这段代码是在AndroidManifest.xml中Google地图导航Glassware的声明

你可以看到在NavigationActivity的<meta-data>标签中

引用到了我们刚刚定义好的

刚才提到过的trigger

voice trigger就讲完了

下次再安装你的apk安装包时

你就能在主界面通过语音和触控两种方式

来启动你的Glassware了

接下来说一下contextual voice menus

语音菜单可以更简单地启动activity

如果你已经掌握了Android中菜单的开发要领  这部分的学习会更简单

Google眼镜中  OK Glass是一条特殊的指令

当你说了一句OK Glass

Google眼镜就会识别出你发出的语音指令

如果可以  还会在屏幕上显示候选菜单项

发出语音指令后

Google眼镜就会选择菜单里的对应项

这跟其他Android设备上菜单的工作方式是一样的

语音菜单项同样要从xml文件中获得

在这段跟导航有关的activity的代码中

在onCreatePanelMenu方法里加载了voice_menu.xml中的内容

然后会在onMenuItemSelected方法中处理语音指令

除了以上介绍的这两个API

开发Glassware时还可以调用Android SDK当中的

RecognizerIntent和SpeechRecognizer

来随时接收用户发出的各种语音指令

我们可以在一个activity中调用RecognizerIntent类  使其能够在Google眼镜上运行

并能够提示用户进行语音输入

这个activity的界面设计

跟Google眼镜其他的应用并无区别

在这段代码中  在MainActivity类中启动了RecognizerIntent

并在onActivityResult中处理intent返回来的数据

如果你想对语音输入做更深入的定制

可以通过SpeechRecognizer直接

调用语音识别服务

你的Glassware可以定义一个识别语音的监听器

用它可以在用户说话时

将声音记录下来

在这段代码中  在MainActivity里创建了一个SpeechRecognizer对象实例

声明了RecognitionListener监听器  并设置了回调函数

有了Android API对语音输入的精确掌控

和Google眼镜专业的调用

再加上我们前面提到的API

你就可以创造出令人眼前一亮的  带有声控功能的Glassware

想要了解更多  请访问我们的网站

并在Google Developers YouTube频道中观看

其他与眼镜有关的视频

谢谢观看