## The picture element for art direction

![video_screenshot](images/QINlm3vjnaY.jpg)

** 视频发布时间**
 
> 2014年10月22日

** 视频介绍**

> Futurelytics Data enthusiast Marcel Laza reveals how to find your most valuable customers. http://www.futurelytics.com.See full playlist at http://goo.gl/SASt1K.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 任皓 | 黄莘 | ——  | [ Youtube ]( https://www.youtube.com/watch?v=QINlm3vjnaY )  |  [ Youtube ]( https://www.youtube.com/watch?v=QINlm3vjnaY ) | 1505050791 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

PETE LEPAGE:你为自己的响应式网站找到了绝好的图片

它在桌面浏览器上看上去非常棒

但是当在手机上看到的却完全没有不行了

由于方向的改变和更小的屏幕等原因  所有很好的细节都无法看到

基于设备独特性的显示不同图片的方法被称为美术设计

图片元素就是为此而设计的

里面是源标签的列表

每一个源标签都包含着一套规则和当规则被触发时使用的图片

你也要包含图像标签

浏览器枚举源列表并且检查规则

一旦它找到匹配的  它将使用那个图像

如果没有匹配的源标签或者图片格式不支持

浏览器使用图像标签达到良好的向后兼容性

我们来看看过程

第一个源标签定义了一个媒体查询

同时检查浏览器的宽度是否大于800像素

如果检查通过  就使用完整尺寸的图像

但是如果第一个源标签不匹配

那就要检查第二个  检测浏览器的宽度是否大于400像素

如果检查通过  浏览器就使用这个图像

当浏览器的宽度小于400像素

或者图片元素没有被浏览器支持

浏览器就会使用被图像标签定义的图像

指定图片元素的样式的方法是

应用css到图像标签上  而不是到图片元素上

这也是你应该定义提示文本和其他所需要的属性的地方

开始吧

现在你知道了如何使用图片元素实现艺术设计

图片元素仅被 Chrome 38 原生支持

但是其他浏览器开发商已经同意实现它了

你可以在确定旧版本浏览器不支持的情况不会发生的前提下使用图片元素

也可以获取一个叫Picture Fill的类库，来支持旧版本浏览器




