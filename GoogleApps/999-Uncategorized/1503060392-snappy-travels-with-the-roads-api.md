
## Snappy travels with the Roads API

![video_screenshot](images/e5YDb-XnDVk.jpg)

** 视频发布时间**
 
> 2015年3月4日

** 视频介绍**

> Mobile apps need accurate visualization of actual roads travelled.The Google Maps Roads API lets you send a bunch of GPS coordinates collected from your mobile phone to Google’s servers and get returned coordinates that snap to roads - letting you create a more accurate visualization of journeys your device has been traveling.By detecting noisy GPS coordinates and discarding them, as well as providing interpolated intermediate points, the returned coordinates can more accurately represent the actual path you’ve been traversing.Mobile apps need to conserve battery power, and reducing GPS sample rates is a good way to reduce power consumption, but if the number of samples gets too low to trace an accurate path, the Roads API lets a mobile app reproduce the actual path travelled without the penalty of power consumption from too much polling.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| weiwei | 贺颂 | 程路 | [ Youtube ]( https://www.youtube.com/watch?v=e5YDb-XnDVk )  |  [ Youtube ]( https://www.youtube.com/watch?v=RSw9_-i5LCI ) | 1503060392 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

很久很久以前 有一个小女孩

和一个小男孩在穿越树林的时候迷路了

他们想出了一个好主意

那就是沿途丢面包屑

这样他们就能找到回家的路了


我是亚历克斯·达尼洛

我想讨论关于手机上的GPS形式的

现代面包屑

当你在移动的时候

有成千上万的 APP 追踪你

当你穿越一片区域的时候

你可以使用 GPS  就像抓住你丢掉的标记踪迹的面包屑一样

比如 你在开车骑自行车或者步行的时候


这太棒了 除了 GPS 的抖动问题

如果你正在沿着一条路走

并且沿途捡到很多面包屑

有可能它们连成的路事实上并不与你正在

走的这条路一样

比如 如果我捡到了10块面包屑

并且尝试把他们连成一条线

事实上它们穿过很多建筑

并且不是我正在走着的路线

这由于几个不同的原因

比如沿途采集的样本太少

或者由于 GPS 收集面包屑的误差

但是使用 Roads API 当你穿过那些面包屑的时候

得到那些事实上捕捉到你走过路径的面包屑后

Roads API 会给你提供服务

得到它们之间的差值

这样你就可以创造出漂亮的

你所走过的 GPS 记录的路径的视觉效果


现在 你可以同时穿过少量的面包屑

比如 假如你穿过100单位个面包屑

并且说 帮我做插值然后生产曲线

你就可以得到大约300个返回值

这样的话 你就可以绘制精确的

你所走的路径的可视化图形

比如 你正在创建一个 APP 去记录你的驾驶路线

这样你就可以和你的朋友们比较

或者假如你正在骑车 

你可能想知道最适合的路线是什么

你的 APP 可以告诉你

Roads API给你完美的方式

在你的手机上呈现可视化界面

通过精确的使用Google Map 的数据

Roads API 同时提供企业客户的元数据

比如 假如你正在创建一个资产追踪器

你可以得到你行驶的道路限制的速度

如果我从 A 点到 B 点

我可以用不同的颜色

来表示行驶的道路所限制的速度

我甚至可以给我的用户们以警告来保证他们的安全

假如他们正在超速行驶的话

我们在这个链接上有一个确切的展示示例

你可以看到源代码 并且可以使用它作为例子

用来创建你自己的 APP 

我们在这个网站上有完整的文档

并且鼓励你们

把它与其他的沿途记录运动状态的 APP 结合

尝试使用Roads API

来给你的用户们展示他们走过的路径

我是 Google 开发者平台团队的亚历克斯·达尼洛

赶紧试试它吧！