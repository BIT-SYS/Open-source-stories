# Python：平平无奇的编程语言小天才

## chapter 0: “人生苦短，我用Python”

相信即使是刚入门的程序员也一定听说过这样一句话：

**人生苦短，我用Python。**


<img src="https://pic3.zhimg.com/80/2ca0db56191f28abcccdbd7f2baf23dd_1440w.jpg" width="250">

这句Bruce Eckel[3]印在T恤上的话被无数喜爱Python的程序员奉为至理名言。随着目前人工智能越来越火，Python凭借着扩展性强、第三方库丰富和免费开源等特点在机器学习、数据挖掘、人工智能等领域独领风骚。在前不久电气和电子工程师协会( IEEE）发布的顶级编程语言交互排行榜中，Python更是超越Java高居首位。

是什么让Python如此受到程序员们的喜爱呢？

我想或许是它的简洁和高效了。

从诞生之初就被评选为最容易上手的编程语言，Python凭借着最接近英语的语法，简单的开发环境，能打字就能写代码，解释执行，众多的第三方库等等等优点杀出了语言大军的重重包围，让饱受加班折磨的程序员们眼前一亮。

在现代社会，似乎掌握了Python，就掌握了打开财富大门的钥匙。

接下来，让我们进一步了解小天才语言Python的诞生。

## chapter 1: 横空出世的python

也许你也曾经听说过Python诞生的故事。

那是在1989年，一个白雪皑皑的圣诞节，阿姆斯特丹的一个小房间中吉多·范罗苏姆(Guido van Rossum)为了打发圣诞节的无趣决定开发一个新的脚本程序，作为ABC语言的继承。

就这样，python在这个寒冷的冬天横空出世，这对于曾获得过计算机和数学的硕士学位的吉多没什么难度，毕竟我们需要承认，有些人就是拥有被上帝亲吻过的脑子。而之所以为这门新语言取名为python(大蟒蛇)据说是因为吉多是一个叫Monty Python的喜剧团体的忠实爱好者。


<img src="https://i2.kknews.cc/SIG=3pst4rb/ctp-vzntr/o276psq04no54poq8o8np0446po3o2r7.jpg" width="250">

这个故事听起来十分简单，似乎只是一个天才程序员的无聊产物。但事实其实并非如此，吉多选择创造Python有他自己的原因。80年代的时候，个人电脑浪潮已经被掀起，然而其配置与今天相比还处于相当低的水平。于是所有的编译起初的核心目的是做优化，以便于让程序在极小的内存条件下仍能运行。这也使得那时的程序员在编程时像计算机一样思考，恨不得榨干计算机每一寸的能力，连指针都被认为是在浪费内存，至于动态类型、面向对象什么的更不用想，因为这些花里胡哨的东西只会让电脑陷入瘫痪。

吉多对此感到很不满。因为即使是像他这样熟练掌握C语言的人，在用C写功能时也不得不耗费大量的时间。同时他还有另一个选择，就是 shell。Bourne Shell作为Unix系统的解释器已经长期存在，它可以像胶水一样将Unix下的许多功能连接在一起。许多C语言下上百行的程序，在shell下只用几行就可以完成。然而，shell的本质是调用命令。它并不是一个真正的语言，不能全面的调动计算机的性能。

所以吉多希望有一种语言可以兼具 C 和 shell 的优点。既能全面调用计算机的功能接口，又能轻松的编程。他本来寄希望于ABC语言。ABC语言是由吉多参加设计的一种教学语言(虽然大部分人都没听说过)。从吉多本人的角度来看，ABC这种语言非常的优美和强大(不排除他带了滤镜)，是专门为非程序员设计的。但很遗憾的是ABC语言并没有成功，吉多认为主要原因是这门语言是非开放的。这次的小挫折让吉多决心在这个新的语言中避免这一错误。同时，他还想要实现ABC中没有实现的功能，比如易于传播、可扩展、可以直接进行IO操作等等[1]。

正是因为有这样的念头作为催化剂，吉多才在寒冷的冬夜里，在那些圣诞树上挂着的五颜六色七彩小灯的陪伴下创造了Python！

所以在一门新语言的创造过程中，它的创作者固然居功至伟，但是我们同样也不能否认当时客观的现实条件对语言发展历史也起着巨大的推进作用！

## chapter 2: python的发展

最初的 Python 完全由吉多本人开发。然而此后Guido同事也迅速爱上了这门新语言。他们不断反馈使用意见，并参与到 Python 的改进中。于是吉多和一些同事构成 Python 的核心团队，他们将自己大部分的业余时间用于hack Python（也包括工作时间，因为他们将 Python 用于工作）。

由于Python实在是太好用了！很快，Python就拓展到了他们的研究所之外。Python将许多机器层面上的细节隐藏，交给编译器处理，并凸显出逻辑层面的编程思考。这使得程序员可以花更多的时间用于思考程序的逻辑，而不是具体的实现细节。这一特征吸引了广大的程序员。Python开始迅速流行起来。

此外，还有两点外界因素使 Python 得到迅速发展。一是硬件性能的提高，当时已进入90年代初，个人计算机开始进入普通家庭，程序员们开始关注计算机和语言的易用性。相比它的兄弟ABC语言因为硬件的性能限制而失败，Python 可以说是生逢其时，正好有机会可以大展拳脚。二是互联网的发展，当时许多程序员以及资深计算机用户已经开始频繁使用 Internet 进行交流。一种新的软件开发模式开始流行：开源。

开放性是 Python 能够发展壮大的根本原因。吉多是一个很谦逊的人。他自认为自己不是全能型的程序员，所以他只负责制订框架。如果问题太复杂，他会选择绕过去，也就是cut the corner。这些问题最终由社区中的其他人解决。社区中的人才是异常丰富的，就连创建网站，筹集基金这样与开发稍远的事情，也有人乐意于处理。吉多维护了一个 maillist，Python 用户就可以通过邮件进行交流。Python 用户来自许多领域，有不同的背景，对Python也有不同的需求。每当用户不满足于现有功能，很容易对Python进行拓展或改造。随后，这些用户将改动发给 Guido，并由 Guido 决定是否将新的特征加入到 Python 或者标准库中。 而这样的特性不仅减少了开发人员本身的工作量，也使得Python得以快速发展[2]。

到今天，Python 的框架已经确立。Python 语言以对象为核心组织代码，支持多种编程范式，采用动态类型，自动进行内存回收。Python支持解释运行，并能调用C库进行拓展。由于标准库的体系已经稳定，所以Python的生态系统开始拓展到第三方包。这些包，如Django，web.py，wxpython，numpy，matplotlib，PIL，将 Python 升级成了物种丰富的热带雨林。

如今 Python 已经进入到 3.0 时代，由于 Python 3 向后不兼容，所以从 2.0 到 3.0 的过渡并不容易。而且目前Python的运算性能仍然低于C++和Java，所以在性能方面仍然值得改进。可以说，即使到了今天，Python仍然有着旺盛的生命力，值得我们去用它来创造一个更值得期待的未来[1]。

## chapter 3: python的版本更迭

python的版本始于1991年。1989年吉多·范罗苏姆开始写python的解释器。1991，第一个python解释器诞生。它是用C语言实现的，并能够调用C语言的库文件。这个最初的版本并不具有版本号，但它已经具有了：类，函数，异常处理，包含表和词典在内的核心数据类型，以及模块为基础的拓展系统。

1994年，python1.0发布，相较于之前的原型，这个正式的版本增加了lambda, map, filter和reduce。之后python1一直更新到了1.6.1版本，随后被python2所代替。[4]

2000年，python2.0发布，加入了内存回收机制，至此奠定了我们现在看到的python语言的基础。也是从python2.0开始，python改变了开发流程，由之前的个人开发转向了社区开发，这使得python变得更加透明，也带来了活跃的社区与旺盛的生命力。之后，python2以每一到两年一个版本的速度进行稳定的更新。到了2008年，python迎来了一次重大的变动——开发组决定开辟一个全新的python版本，用以彻底解决python2遗留下来的一堆麻烦。也正是出于这种考虑，python的这次版本更迭使用了极为罕见的不后向兼容的模式，这就意味这python2的一些语法与特性不会在新的python版本中得到支持。于是诞生了python3，以及困扰了python社区十年之久的python2与python3不兼容问题。

python3相对于python2的主要区别包括：  
- print。python2中的print语句在python3中被改为了函数
- 编码。python2默认使用ASCII，而python3默认使用utf-8
- 除法运算（/）。在python2中，整数/整数=整数，小数/小数=小数。而python3中，整数/整数也可以是小数。
- xrange。在python2中，存在xrange与range两个函数创建迭代对象。但是xrange返回生成器，range返回列表。在python3中，range使用了python2中的xrange模式，而xrange在python3被删除了。
- 不等运算符。python2中有两种不等运算符：<>与!=，python3只保留了!=
- 很多模块的名称被修改了。
- 数据类型。python3去除了python2中的long类型，现在只有一种整数类型——int。但实际上，这个int的机制是与python2中的long相同的。
- map与filter。python2中，它们都是内置函数，输出结果是列表。而到了python3，它们变成了类，返回的结果也变成了可迭代对象。[5]

但是在2008年python3发布之后，很多用户的python2代码因为python3不支持python2的问题无法顺利升级到python3。于是2010年，python2又发布了一个过渡版本——python2.7，并一直保持更新。2018年，吉多·范罗苏姆宣布python2将在2020.1.1到达EOL（end of life 寿终正寝）。这个日期之前的最后一个python2版本是2.7.17，在它之后到2020.1.1的所有问题，将依然被开发者接受，并在2020年4月的2.7.18中解决，这将是python2的最后一个版本。[6] 就在本文写作几天前（2020.4.20）python2.7.18发布，至此，python2画上了句号。

但python3仍在茁壮成长。自2008的python3.0开始，每一到两年更新一个版本，并一直保持小版本的及时更新。python3的开发者们在这上面也展示出了饱满的热情，每次的版本更新，除了修补发现的问题，还会增加一些新功能（比如3.8的海象运算符）。到本文写作时（2020.4.25），最新的python3版本是3.8.2，同时3.9正在开发中。


##chapter 4：IronPython和它的创始人吉姆
IronPython是一个与.NET框架紧密集成的Python编程语言的一个开源实现。IronPython能够使用.NET框架和Python库，并且其他.NET语言可以很容易的使用Python代码。IronPython是.NET框架的一个优秀补充，为Python开发人员提供了.NET框架的强大功能。现有的.NET开发人员也可以使用IronPython作为一种快速且富有表现力的脚本语言，用于嵌入、测试或从头开始编写新的应用程序[7]。  

IronPython是在动态语言运行时(DLR)之上实现的，DLR是一个运行在公共语言基础结构之上的库，它为动态语言提供动态类型和动态方法分派等功能。

IronPython完全是用c#编写的，尽管它的一些代码是由用Python编写的代码生成器自动生成的。

吉姆（Jim Hugunin）创建了这个项目，并且直到2006年9月5日发布的1.0版本，他都一直积极参与其中[8]。  
![Jim Hugunin headshot](https://github.com/BIT-SYS/Open-source-stories/raw/master/img/Jim_hugunin_headshot.jpg)  

2010年，微软放弃对IronPython的投资，吉姆离开微软加入了谷歌。在吉姆的个人网站中，他表示“将微软对于IronPython的决定是我离开微软的催化剂，但不能算是原因”。他还表示，在微软有一个“开源代码和社区保持健康的关系”是“可能的”，但“感觉就像把方钉入圆孔”。  

根据领英的资料，吉姆于2013年5月离开了谷歌。  

2017年12月，吉姆发布了一个名为Artful Physics的布料模拟器测试版。然而，Patreon和艺术物理社区的帖子表明，他从2018年1月起就缺席了[9]。


## Reference

[1]https://blog.csdn.net/laagyzz/article/details/78802403  
[2]https://www.cnblogs.com/vamei/archive/2013/02/06/2892628.html  
[3]https://baike.baidu.com/item/Bruce%20Eckel/3646582?fr=aladdin  
[4]https://www.cnblogs.com/xincai/archive/2017/06/21/7058551.html  
[5]https://www.runoob.com/python/python-2x-3x.html  
[6]https://mp.weixin.qq.com/s/ql_lV9xzRFtRezcRGTpdqg  
[7]https://ironpython.net/  
[8]https://en.wikipedia.org/wiki/IronPython  
[9]https://en.wikipedia.org/wiki/Jim_Hugunin