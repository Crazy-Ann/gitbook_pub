## Drive Android API  

![video_screenshot](images/1rUZmkifDPk.jpg) 

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍** 

> Jennifer King shows you how to Cloud-enable your app without writing a single line of networking code using the new Google Drive API for Android. Learn how you can interact with the files and folders stored in a user's Drive from your app with seamless offline support.

** 视频推介语 **

>  暂无，待补充。

### 译者信息 

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| ----|----|----|----|----|----|----|
| 點墨 | Wallace4ever | -- | [ Youtube ]( https://www.youtube.com/watch?v=1rUZmkifDPk ) | [ Youtube ](https://www.youtube.com/watch?v=x437FamBHXk) | 1504010485 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator ) |


### 解说词中文版：

大家好  我是 Jen King  Drive Android API的

技术主管

今天我来向大家展示一下

如何将Google Drive集成到Android应用中

Drive的API是Google Play服务套件的一部分

这意味着只需在应用中添加少量的代码

便可实现这些API的功能

并且可以在几乎所有的Android 2.3.3及以上系统的设备上运行

对用户来说集成Drive有很多好处

是不无道理的

文件自动备份到云端

可以在包括网页端在内的各种设备上访问

在移动设备和网页端  使用Drive应用可以查看及修改这些文件 

甚至离线时也可以

好的  我们开始吧

我会用一个收据收集的示例应用

来演示如何整合Google Drive

这个应用允许用户对收据拍照

并将它们存储在Drive来管理自己的开销

为了使用Drive Android API

首先需要在开发者控制台创建一个条目

以将你的应用注册为一个Drive应用

控制台会要求提供应用的包名和

签名证书的指纹  

以便Drive API验证应用

在开发者控制台创建一个项目ID

可以让你构建跨安卓  iOS  和网页端的

多平台应用

这些应用可以共享使用一个项目配置

项目注册好之后  就可以为应用添加Google Play服务套件的支持

以开始使用Drive Android API

在整合Drive之前  我们的应用只是

将收据保存到本地设备

也就意味着其他设备很难访问它们

如果我丢失或弄坏了我的设备  该数据也可能会随之丢失

然而  使用Drive Android API

备份这些收据是很容易的

要做到这一点  我们会通过Drive API

创建一个新文件

而Drive API会将图片字节数据同步到服务器

我们需要将收据图片数据写到一个Contents对象

然后拿它来创建一个新的Drive文件

现在  我们将所有的收据图片都放到用户的根目录  

换句话说  放到我的云端硬盘中

要保存新文件  我们需要在目标目录下调用createFile

并传入刚才创建的包含图片数据的

Contents对象

调用createFile会返回新文件的Drive ID

现在收据便可自动上传到用户的Drive中

使用户能够在网页端

查看及组织它们

下一步  我们来改变我们的收据清单

这样就需要从Drive API

而不是本地文件系统请求收据文件列表

要做到这一点  我们会在收据应用可以访问的  

用户的云端硬盘即用户目录下查询所有文件

该查询使用的是本地的Drive数据库  而非服务器

所以离线时它依然可以正常工作

Drive Android API会自动同步

其它设备所创建的文件的元数据

要想使我们的收据列表显示与

与Drive中的数据保持同步

需要列表视图的适配器使用查询方法

所返回的元数据缓冲区对象

对于列表里的每个文件  我们使用title字段生成一个条目

最后  当用户从列表中打开它时  

我们需要显示其收据图片和描述信息

要显示收据图片  需使用DriveApi.getFile

获取收据的Drive文件

并以DriveFile.openContents打开

如果文件内容在设备上已经存在 

这种打开文件的方法将立即返回所需内容

否则  Drive Android API就会

从服务器获取内容

现在  应用就可以做到如之前所说的

额外好处了

即用户可以在任意Android设备或网页端

查看所有的收据信息

另外还有三个很酷的功能

可以给我们带来更好的用户体验

固定文件  文件选择器  以及应用文件夹

第一点  你可以使用  设置固定  API

让你的用户将收据保存到本地  固定文件  以脱机使用

该API会确保该文件的内容留存在本地设备上

并保持最新  当然是在网络通畅的情况下

为了让用户使用此功能

我们会在  查看收据  页面添加一个曲別针状按钮

从而让用户选择是否将文件保存在本地设备

第二点  我们目前是将所有收据保存到了用户的

‘我的云端硬盘’文件夹

但是  能不能让我们的文件组织更清晰一点呢

我们可以启动一个  云端硬盘文件选择器

来让用户选择保存收据的

文件夹

一旦用户选择了某个文件夹  我们便将该选项保存到本地设备上

而且我们每创建一个新的收据

都会把它放到之前所选择的文件夹里

最后  如果可以将文件夹设置项

在多个设备保持一致就更好了

当然我们可以将设置项存储在Drive的一个文件里

就像存储收据一样

不过这个文件会弄乱用户的Drive文件结构

这总是不好的

所以Drive最后一项功能就来了

应用文件夹是一种特殊类型的文件夹

在这里你可以存储只有你的应用可以查看和管理的文件

该文件夹仍然使用用户存储配额

并且可以在用户不再使用你的应用时

清除文件夹里所有的内容

但之前的那些收据文件依然存在

现在  让我们回顾一下我们刚才讲的东西

我们主要说了一个应用

它将所有的数据存放在本地设备上  并加入了自动备份  跨设备文件同步

离线支持  以及应用配置同步等功能

你也可以将这些功能添加到你自己的应用中去

所以  开始使用Drive Android API吧

你可以在developers.google.com/drive/android找到更多资料

我是 Jen King  期待你用Drive Android API

做出来的产品哟

