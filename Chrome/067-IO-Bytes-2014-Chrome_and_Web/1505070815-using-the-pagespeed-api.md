## Using the PageSpeed API 

![video_screenshot](images/vPfz2VwIryk.jpg) 

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> How to integrate the PageSpeed Insights API into your work flow, understanding what it can do and how it can help you to ensure you've got a great mobile experience.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 韩淼 | 素年待锦 | -- | [ Youtube ]( https://www.youtube.com/watch?v=vPfz2VwIryk )  |  [ Youtube ]( https://www.youtube.com/watch?v=9kYH7ZhCS0k ) | 1505070815 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

hi 我是Pete  Google的一名开发人员

我们都知道一个简洁的网页很棒

它意味着用户满意度与评价的提升

而在手机端的体验速度很重要

特别是如今每人总是处于匆忙中

PageSpeed Insights是一个很赞的工具

你可以用它去提高产品的性能

当你用PageSpeed Insights刷新一个页面

它会对页面进行评估

并以性能和用户体验为依据打分再发送给你

这些都以预先设定的标准和试验为基准

要进行一个快速简洁分析

你只需点击屏幕上的链接到PageSpeed Insights service

让我们以Web Fundamentals

为例看它是如何工作的

我会进入URL  连接到Analyze按钮

几秒钟之后  PageSpeed报告返回调查结果

这个页面  我们为100的速度打了70分

还行  但还有很大的提升空间

它给我们了一个需要遵循的标准列表

在这个页面中  它建议我们消除

render-blocking CSS和脚本

在此例中  这是我们的原始CSS文件

一个CSS文件装载一些专业的文字

它也告诉我们  我们应该看看一些文件的缓存文件


它显示出一些文件被储存了60分钟

很显然 我们想提升那个数字

我们已经符合了8条规则  这些都不用调整

并且页面的权重已转向

对压缩和消减的JavaScript  HTML

CSS  和图像优化

上面的内容已经确保优先顺序

并且这些响应得很快

很好 现在处于良好的状态

我们的用户体验标准也得到了相似的报告

它看起来像页面有两点  因为

上面的一些对象靠得太近

另外  这个界面很好

他不需要任何的插件程序  这个视口

装配很合适  并且内容都可以去适应

所有的字体大小适合去阅读

它像知识手册一样全面  分析也一步到位

但是你可以更加深入

你可以通过PageSpeed Insights API直接将PageSpeed整合到

你的工作进程中

它使用包含了三个参数的REST API

我们希望去测试的URL  定义工程的API

并且  顺便说一下

这并不是我真正的API 密码  所以不要尝试

还有策略或者是桌面或手机

你所希望再去测试

你可以学到其他可选择的参数

在这个记录中

现在如果你该没有任何API密码

你需要去Google Developer Console激活


并获得你的密码

PageSpeed Insights API以JSONObject的形式返回结果

它包含了服务回应代码  最终的URL以及分数

他也包含页面统计例如总共的字数

每个资源下载和主机的总数

和回应的大小

最后  所有规则都被测试过了

每一个PageSpeed 产生冲击的数字

它指示出重点或者优先的实施步骤

相对于其他规则设计规则

例如  如果启用压缩

可以节省一个兆字节  而优化的图像将节省500k

然后启用压缩规则所影响价值的

是优化图像的

两倍

你可以从命令行查询URL

还有更好的  实现自动化

Grunt使命令行测试非常简单

The Grunt PageSpeed plug-in会简单地

测试页面的有效利用率并且返回报告

该份报告包含页面属性和个人统计的结果

如果PageSpeed评分低于指定的阈值

那么Grunt测试失败

经常使用Cron job测试你的网站  

或者其他计划任务并且保存结果

渐渐地 你可以使用PageSpeed Insights检测你的网站

单独观察时小的改变

可能不会有太大的不同 但是随着时间发展  这些数量会

增加  帮助你去回归

或者引起你注意你可能已经错过的趋势

在你的发展记录里加入PageSpeed Insights

你可以通过良好的测试确定你的页面

表现和用户体验

并且你可以在它们成为问题之前观察到趋势

开始吧  测试你的页面

然后加入PageSpeed Insights到你的工作流程

感谢观看  去创建一些美好的东西吧

