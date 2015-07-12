## How I: Use BigQuery to find my most valuable customers 

![video_screenshot](images/K2NN_XzAdr4.jpg) 

** 视频发布时间**
 
> 2014年10月22日

** 视频介绍**

> Futurelytics Data enthusiast Marcel Laza reveals how to find your most valuable customers. http://www.futurelytics.com.See full playlist at http://goo.gl/SASt1K.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 田源 | 任皓 | -- | [ Youtube ]( https://www.youtube.com/watch?v=K2NN_XzAdr4 )  |  [ Youtube ]( https://www.youtube.com/watch?v=XkIxDyEe0Nk ) | 1504070573 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |


### 解说词中文版：

哈罗

我叫Marcel  在创业公司Futurelytics

是个数据分析狂

今天  我会向大家展示如何使用BigQuery

找到最有价值的用户

二八法则的一个基本观点是

可以为你带来80%的利润的最有价值客户

占总体的20%

在这个例子中  我会向大家展示

如何使用BigQuery找到维基百科上最有价值的

贡献者

数据来自其它的公开数据集

BigQuery控制台里可以使用

所以你可以使用基本的SQL操作

为了在维基百科的数据集合上二八法则计算

我们首先需要做一个基础计算

得出每位贡献者、内容创建者

编辑过的页面数

执行这个简单查询

然后我们能看到贡献者ID和

编辑过的页面数

这种基本的运算方法被用在二八法则的

高级计算中

这个  这个  这个  还有这个

这有我们开始使用过的基本运算

然后我们计算了每个贡献者所处理的累加值

这样我们就可以将贡献者划分为两组

分别是特别重要的贡献者或者

是一个编辑了少量页面的贡献者

结果会显示一些累加总数

和每个贡献者的贡献总量

通过这些计算  我们可以

将贡献者划分到特定的分组中

在这个例子中  我们有了基础查询  和第二个查询

来帮助我们计算累加的总指标

这是个错误的查询

应该用这个

再一次  在这个查询中  我们用到了最开始使用的

基本的查询  和第二个查询

通过他们我们可以计算累加总数

而且我们很关注维基百科中有多少重要的贡献者

所以我们会把这个查询放到

另外一个里  这样我们可以

计算每个分组中的贡献者数

结果是维基百科里共有

26000个重要的贡献者  有4400000少量贡献者

从二八法则计算中  我们发现了

最有价值的贡献者数达不到20%

8%的贡献者

为用户提供了维基百科中80%的有价值的信息

在我们最初创建Futurelytics的时候用到了这个基本的计算

对我们来说  要找到最有价值和次有价值的客户

这是最简单的一种方法

