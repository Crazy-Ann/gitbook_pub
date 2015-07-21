## Responsive images today

![video_screenshot](images/vpRsLPI400U.jpg)

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> For developers who want to use responsive images today, what can they do? We'll cover the current state like picture, img src, srcset, etc and include suggestions around art direction.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 韩淼 | 素年待锦 | —— | [ Youtube ]( https://www.youtube.com/watch?v=vpRsLPI400U )  |  [ Youtube ]( https://www.youtube.com/watch?v=4MbISD5Q4go ) | 1505070819 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：


我是Pete  一名Google开发者


几乎在每一个网页里图像都是不可分割的一部分


并且是消耗下载字节最多的一部分


今天我要展示几个技巧


你可以用它在页面上为设备提供相配的图像


而且不需做太多的工作


首先  先通过css看一下后端图片服务器


今天你可以使用的技术是


结合后端属性


使用查询下载有条件的图像


这些都依据屏幕分辨率  视口大小等


在之前的例子中  当窗口大小


小于500像素  它只适用于手机的图像


当窗口像素超过500像素时


会使用媒体查询  加入一张New York City 的照片


到后台


并非用于在手机上显示的图片


它会在平板上显示图片


媒体查询也适用于


以设备像素比为基础的设备


它可以显示不同的像素从1x到2x的显示


Chrome  Firefox和Opera都支持标准的


(min-resolution: 2dppx)属性


而且速度会快很多


Safari和Android浏览器都要求


供应像素语法dppx单元


记住  这种模式仅仅适用于


设备为手机查询时


所以你通常要提供一个回退的东西


这可以保证图像总是被下载


最近Chrome和Safari都载入新的CSS image-set


函数  能够复杂图片文件的提供简单化


允许浏览器根据设备选择最匹配的图像特征


例如


一个2x对应2x显示或者1x图像对应1x显示


它的语法很简单


一份图像列表声明


由URL字符串跟随者图像分辨率组成


为图像设置功能的支持


仍旧是新的  随着时间推移


需要WebKit供应的前缀


除了下载正确的图像


浏览器会相应的衡量


浏览器假设2x图像是1x图像


两倍大  并且会衡量2x图像


它以正确的大小出现在屏幕上


现在对于图像与标记  仍没有什么选项


画面元素来到  但还没有下载


在Safari和Chrome中  你可以使用新的srcset属性


srcset元素可以提高


图像元素的表现  为不同设备特征提供


复杂图片文件更为简单


语法资源设置几乎与CSS image-set函数


设置一样  为图像声明建立一个以逗号间隔的表格


它包含了


跟随着图像分辨率的URL字符串


因为srcset能够很简单的为图像元素加入新的属性


如果浏览器不支持srcset


它简单的忽略它并且使用根源属性


它同样也会简化建立一个polyfill


而且相当富余


在一些情况下  图片可以


用CSS代替或者其他浏览器


圆角  梯度  文字阴影  阴影框


甚至映像都可以用CSS做成


而不需要下载图片


当一个人终于传递了16  20或者30


或者任意一个显示


你将不需要再创建一个新的图片文件


为你的网站加一个响应图片很简单


至于背景图片  我已经向你展示


如何使用手机查询或者近期的


图像设置功能


通过图片和标记  图像也会很快来到


现在你可以使用srcset属性


也会有更多的能力来到


了解更多响应图像


在Web Fundamentals网站点击图像部分


或者点击屏幕上的链接


好的


在这里


完美


感谢观看


去创建完美的东西吧







