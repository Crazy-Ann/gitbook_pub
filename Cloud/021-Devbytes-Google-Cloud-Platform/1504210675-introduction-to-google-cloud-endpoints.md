## DevBytes: Introduction to Google Cloud Endpoints

![video_screenshot](images/A7yMmvrpMJc.jpg)

** 视频发布时间**
 
> 2014年3月21日

** 视频介绍**

> Do you need a server for your mobile or web clients? Learn how you can use Google Cloud Endpoints to create a server API and auto-generate client libraries for Android, iOS, and web. The communication between client and server is handled for you on secure Google infrastructure. In addition, your service scales easily and robustly to meet your users' needs, without you needing to worry about server maintenance tasks.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 韩淼 | 葛伟 | —— | [ Youtube ]( https://www.youtube.com/watch?v=A7yMmvrpMJc )  |  [ Youtube ]( https://www.youtube.com/watch?v=yDtDudTOFqs ) | 1504210675 | [ 加入 GDG 字幕组 ]( {{ book.host }}/join_translator )  |



### 解说词中文版：

告诉我你是否经常这样

在你有有关app很棒想法并且想去实现它

你所想到的是去做运行平台以便在它上面开始工作

当你开始创建它时  很快

你就会意识到  你需要一个后端或是一个服务器

去完全实现你的设想

你打开浏览器开始搜索

如何为一个移动或是网页app创建后端和服务

哦  出现的是百万数量的  所有类型的

文章和论述线索之类的搜索结果

并且它会覆盖掉

如何将这些技术整合起来

好消息是  有了Google Cloud Endpoints

你可以控制很多复杂的事情

它的工作流程很明确

你创建的后端可以被Android  iOS和网络客户端

所兼容

之前  我在Google Keep团队作为一名志愿者

并且因为今天我讲的这些问题被发掘

在一个新的项目中

通过多客户端连接后端

这就是我为什么帮助你尽可能快的使你的

服务生成并运行

在服务器中  你可以很轻松的定义你的API

并且嵌入Cloud Endpoint注释

这里有一个令人惊叹的工具可以自动生成客户端

你可以加入到你的app中

运行客户端代码调用你的API

和服务器逻辑关于API被调用后的工作

之后  两者之间其他的事情都被Cloud Endpoints执行

一段时间后  你的服务API会进步发展g

这就是Cloud Endpoints可以减少

意外错误的地方

因为它会自然增加客户端库

当你最新版本需要减少客户端

我们会帮你平稳的升级

现在Cloud Endpoints中API的发展

使它成为可能

不同的API版本可以共存

你可以平稳的完成这些改变

在这个例子里  新的客户端可以与V2 API创建联系

此时你旧的客户端运行很慢

直到你不再支持旧的V1 API

我还想提醒一下  我们讨论的后端服务

完全在Google App Engine上运行

它是Google Cloud Platform的一部分

你不仅可以得到一个在Android iOS和

网页客户端兼容的后端  还可以

享有其他产品和服务所提供的

优点

App Engine能很容易形成规模

如果你得到更多的浏览量  Google自动的

为你运转更多App Engine程序

之后当你的浏览量超过顶端

我们会去掉你不再需要的程序

你不用再提前估计需要的资源
You don't need to t、rouble yourself

为你自己找麻烦  这样很棒

作为一个额外的福利  Cloud Endpoints

适应网络管理工具  例如这个API Explorer

它允许你与你所有的API进行交互

如所见  你可以创建一个请求

之后看回应是什么

如果你希望概览

服务对你的用户来说是否健康

在这个仪表上你可以检查图标

用QPS  吞吐量和错误率

如果你希望得到更多细节的数据  你可以连接到记录

但对发展来说是足够了

Cloud Endpoints实际上能对你的用户产生什么类型的影响

用户希望app运行很快

不需要长时间加载

这并不理想  如果你有横跨半个地球的用户

然而他们不希望使用的服务

位于你底层的

相反  你可以利用Google的全球基础设施

我们在全世界都有数据中心

并且我们会把请求尽快发给适合的数据中心

现在  用户们还关心减少网络的使用

这会影响他们的账单  同时

他们也想减少电量的消耗

因此  一但我们加载数据

我们通过网路高效的传递它

现在我们知道  用户也想保证

他们的数据在存储和传输是尽可能保密

因此我们所有的请求都是通过HTTPS传递

我们支持OAuth 2.0

它可以认证和授权用户

访问适当的数据

如你所见  Google Cloud Endpoints

是一个简单的方法去建立一个被

Android  iOS和网页客户端兼容的后端

如果你现在浏览器还开着

你可以搜索一下Google Cloud Endpoints

或者你可以点击这儿的链接

当你再有好想法的时候  你就知道该怎么做了




