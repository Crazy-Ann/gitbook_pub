
## DevBytes: Web Components - Overview

![video_screenshot](images/T5y_lmLngAk.jpg)

** 视频发布时间**
 
> 2014年6月25日

** 视频介绍**

> Web Components are a set of technologies that changes the way you develop web apps entirely. By making components scoped and reusable in standardized way, your web development will step up to the next level.This video explains the benefit of using Web Components, how to use them, and what each technologies are like.

** 视频推介语 **

>  暂无，待补充。


### 译者信息

| 翻译 | 润稿 | 终审 | 原始链接 | 中文字幕 |  翻译流水号  |  加入字幕组  |
| -- | -- | -- | -- | -- |  -- | -- | -- |
| 黄玄 | 任皓 | —— | [ Youtube ]( https://www.youtube.com/watch?v=T5y_lmLngAk&list=PLOU2XLYxmsIJkA_W95NDrjdkk3dR6Jq4w&index=1 )  |  [ Youtube ]( https://www.youtube.com/watch?v=8WWmY67PoUk&index=22&list=PLvivLNHqjoowcHLv6e2X2TpT08IDKOV1H ) | 1504250709 | [ 加入 GDG 字幕组 ]( http://www.gfansub.com/join_translator )  |



### 解说词中文版：

嗨

我叫英二  是一名来自 Google 的开发者布道师

今天  我将和大家笼统的介绍一下Web Components

Web Components 是一套新兴的规范

它可以完全改变你开发网页应用的方式

这套规范允许你在开发网页应用时创建和复用 UI 组件

这套规范允许你在开发网页应用时创建和复用 UI 组件

让我们来看看在今天你要如何去创建一个 UI 元素

同时了解使用 Web Components 能如何改善这个过程

这里有一张很好看的图表

你会如何使用 HTML CSS 和 JavaScript 来创建它呢

如何你从零开始  那么工作量很大

为了帮助我们做这个图表，我们可以使用 Google Visualization API（可视化）

首先  载入 Google JavaScript 库以使用这些API 

然后  添加 div 标签到 body 中作为占位符

现在  使用 JavaScript语句 通过加载 Visualization API 来初始化类库

现在  使用 JavaScript语句 通过加载 Visualization API 来初始化类库

接着，在回调函数中设置值和一些可选项

最后，指定用来放置图表的 DOM（文档对象模型）元素


现在，让我们进入 Web Components 的方式

看看它如何剧烈的改变了我们创建一个图表的方式

看看它如何剧烈的改变了我们创建一个图表的方式

使用 Web Components，你需要做的第一件事

就是载入 Google Chart Component（图表组件）

为了使不支持的浏览器也能正常表现

你还需要加载一个开源的polyfill（提供兼容性的代码）  platform.js 

然后添加一个 Google Chart 标签并且把你想要的属性填进去

就搞定了

注意到两种方式的区别了吗

是的

第一种是使用 JavaScript 的指令

而第二种则是使用 HTML 标签的声明

声明方式可能看上去更容易处理一些

但最大的不同并不在难易

而是当使用那些 API 时，开发者需要很多潜在的知识

而是当使用那些 API 时，开发者需要很多潜在的知识

在最初的那个例子中  你首先需要理解 Google JavaScript 库是如何工作的

在最初的那个例子中  你首先需要理解 Google JavaScript 库是如何工作的

然后你才可以学习如何运用 API 来控制它

相反  Web Components 使用 DOM API 

这是大多数 Web 开发者都非常熟悉的

这是大多数 Web 开发者都非常熟悉的

这样你就可以直接从学习如何使用属性和 API开始

这个差异看上去很微妙  但是当你使用其他 UI 类库时  你就会发现它的好处

这个差异看上去很微妙  但是当你使用其他 UI 类库时  你就会发现它的好处

比如 jQuery UI  Bootstrap  Closure Libraries 等等

它们全都使用了不同的方式

以至于在实际开始使用之前  你先要学习他们

使用 Web Components 还有诸多其他好处

让我们一个个来看

有作用域

由于 Web Components 的样式和标签是有作用域的

引入的组件并不会损害到你网页的其他部分

现有的库中存在这么一个情况

你用到的类名或ID可能会和库中已有的重叠

你用到的类名或ID可能会和库中已有的重叠

使用Web Components  所有标签和 CSS 的作用范围仅限于该元素内部

这意味着 CSS 被捆绑在了组件上

而不会泄漏出去影响到父document

这同样防止了父document的样式意外影响组件

这同样防止了父级元素的样式意外影响组件

复用性

因为 Web Components 是有作用域

并且与网页其他部分解耦的

你可以在网页的不同部分甚至另一个站点使用相同的组件

你可以在网页的不同部分甚至另一个站点使用相同的组件

不仅如此  你还可以与社区开源分享你的元素

不仅如此  你还可以与社区开源分享你的元素

使得任何人都可以从你的工作中获益

分离性

因为 Web Components 是有作用域的

你可以将 UI 组件的开发从主功能的开发中解耦出来

开发者们因此能够独立地进行 UI 组件的开发工作

而无需担心或者注意网页其他部分的实现细节

而无需担心或者注意网页其他部分的实现细节

可以看到，组件的维护因为分离也变得更加容易了

可以看到，组件的维护因为分离也变得更加容易了


Web Components 听上去是服务或使用 UI 组件的绝佳解决方案

Web Components 听上去是服务或使用 UI 组件的绝佳解决方案

那么我们实际中要如何创建我们自己的组件呢

Web Components 由四个核心技术组成：

templates  Shadow DOM  Custom Elements  与 HTML Imports

让我简短地介绍一下它们都是什么样的

Templates（模版）允许你定义惰性的样板文件

用于描述你在 HTML 中重复使用的标签

因为模版中的内容是惰性的

直到它们被送入页面里

它们并不会请求图像或者执行脚本

Shadow DOM (后台DOM)允许你把有作用域范围的 HTML 标签

和 CSS 文件关联到现有的 DOM 元素上

由于 Shadow DOM 是被封装起来的

其样式并不会影响到任何外面的元素

Custom elements（自定义元素）允许你定义并且注册

一个自定义的 HTML 元素就好像它是原生的一样

HTML Imports（导入）允许你加载多个资源

比如 JavaScript, CSS 和附加的 HTML 文件

通过加载一个单独的 HTML 文件来实现

组合所有以上技术就会像这样

首先  准备一个不同于主要 HTML 文件的 HTML 文件

定义并且注册自定义元素

关联 Shadow DOM到上面

使用模版以提供 Shadow 的内容

最后  使用 HTML Imports 导入这个组件 HTML 文件

现在你应该对 Web Components 有了个基本的概念

我将继续发布一系列有关 Web Components 特性的视频

让你可以继续学习如何使用它们

在此期间  列在这里的文档和资源都可以帮助你学习更多

都可以帮助你学习更多有关 Web Components 的知识

所以你可以去看看它们

好啦

感谢您的观看

我们下期再见




