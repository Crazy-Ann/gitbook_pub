## Game On! - WebP for Game Devs

![video_screenshot](images/1pkKMiDWwpM.jpg)

** 视频发布时间**
 
> 2014年11月12日

** 视频介绍**

> For many game devs out there, PNG Image files are a backbone of their development process, but they also come with some unintended side effects; mainly that they create bloated asset footprints that increases the time it takes for a user to get your application. In this video, we discuss how WebP is an available drop-in solution for games that will destroy your bloated-game-woes.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| eternity | 段威 | -- | [ Youtube ]( https://www.youtube.com/watch?v=1pkKMiDWwpM )  |  [ Youtube ]( https://www.youtube.com/watch?v=2EkDzLJgdXI ) | 1504030547 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

COLT MCANLIS：对于许多游戏开发者来说

PNG图像文件是开发过程中不可或缺的一环

但它们也会带来一些意想不到的副作用

我的名字叫Colt McAnlis

对于贴心的开发者来说  

他们更关注用户的带宽和下载快慢  

PNG文件不一定是游戏资源的最好选择

可是PNG文件在移动开发中随处可见已成为一个现象

在分析了谷歌Play前1000名游戏之后

我们发现PNG文件占据了所有游戏材质的75%之多

这很说得通啊 对吗

因为开发者们都是大忙人嘛

PNG文件容易使用  支持透明度

支持压缩存储  还可以跨平台使用

但是由于移动端下载时长的特殊性

用户常常会接收不到  还有流量上限的问题

你的应用是大是小至关重要

PNG文件当然没法改善现状

对那些寻求减少图片材质

所占游戏包大小的开发者而言

WebP图片格式可谓一个完美的替代

WebP提供了游戏开发者喜欢PNG的大部分特性

也就是说  透明度啊  跨平台啊

无损压缩等

但它更进一步  还支持有损压缩

这意味着你可以得到更小的文件

WebP能无缝接入开发流程

只要有了Adobe Photoshop，GIMP，ImageMagich等对应的插件即可

还有  命令行转换工具允许你

一边开发一边把资源打包

程序员们有福啦：）

在游戏里用到WebP十分容易  

在你现有代码的基础上加一个C++的库  调用就好

允许你在移动端或者PC端上使用

也可以在web页面上使用

为了更直观地感受其有损压缩的可靠性

WebP团队跑了一些测试

来看一下它比PNG强在哪里

他们在一个资料库里面测试了1000张图片

这个图表显示了常规结果

你可以看到最常用的PNG文件

被列为一条数值为1.0的绿线

同时清晰地看到有损和无损两种压缩模式下

WebP文件总是能更小

在最后一点尽管出现了奇怪的翘起

那是由1*1像素的图片引发的

这么好用的WebP总该有点Bug的吧

不管怎样  现在就是想告诉你

WebP它有高级的处理技巧

以下非常重要  因为在你的游戏里

用一种压缩方式处理可不会一劳永逸哦

低品质位图和正常位图是不一样的

和带alpha通道的位图也不一样

和高度透明的图像就更不一样了

这说明要找到图像质量和大小的平衡点

也就是要找到

适合每个图片的压缩类型

但是  在游戏开发里这样做是不切实际的

怎么做呢  首先根据它们的用途分门别类

这通常也决定了它们看起来的样子

然后  你可以把一类一类的图组

与它们特定的压缩形式一一配对

你的设计师们在随便一天的下午

简单花几个小时就能搞定了

噢  当然还要写一个文档

来记录某些最特殊的图片

它们的压缩形式可能和其所在组别的还不一样

相信我  你的设计师肯定会因为你这么贴心而感动

现在  是时候指出PNG和WebP文件

都不是GPU格式

也就是  当你把他们解压到主内存里面

它们将会全部以32比特/像素来驻留在GPU中

本来有一些支持GPU的压缩格式

像DXT，ETC，PVR和ASTC

都以压缩形式存在于磁盘中

这意味着你需要考虑用WebP去支持GPU格式

因为某些图片材质可能会支持

这样的话  你既优化了你的游戏包大小

也优化了GPU使用强度

好啦  开始用WebP吧

快跳去开发者网站  为你的游戏来一发C++ SDk

读一读在线文档

另外一定记得注意alpha blending的相关信息

它可能会在游戏里引发一些问题

去看我另一视频“Don't Alpha That Pixel.”就好啦

WebP能在应用里完美地取代臃肿的PNG文件

所以去干活吧  压缩你的材质  开发出更好的游戏


