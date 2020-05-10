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

就这样，Python在这个寒冷的冬天横空出世，这对于曾获得过计算机和数学的硕士学位的吉多没什么难度，毕竟我们需要承认，有些人就是拥有被上帝亲吻过的脑子。而之所以为这门新语言取名为Python(大蟒蛇)据说是因为吉多是一个叫Monty Python的喜剧团体的忠实爱好者。


<img src="https://i2.kknews.cc/SIG=3pst4rb/ctp-vzntr/o276psq04no54poq8o8np0446po3o2r7.jpg" width="250">

这个故事听起来十分简单，似乎只是一个天才程序员的无聊产物。但事实其实并非如此，吉多选择创造Python有他自己的原因。80年代的时候，个人电脑浪潮已经被掀起，然而其配置与今天相比还处于相当低的水平。于是所有的编译起初的核心目的是做优化，以便于让程序在极小的内存条件下仍能运行。这也使得那时的程序员在编程时像计算机一样思考，恨不得榨干计算机每一寸的能力，连指针都被认为是在浪费内存，至于动态类型、面向对象什么的更不用想，因为这些花里胡哨的东西只会让电脑陷入瘫痪。

吉多对此感到很不满。因为即使是像他这样熟练掌握C语言的人，在用C写功能时也不得不耗费大量的时间。同时他还有另一个选择，就是 shell。Bourne Shell作为Unix系统的解释器已经长期存在，它可以像胶水一样将Unix下的许多功能连接在一起。许多C语言下上百行的程序，在shell下只用几行就可以完成。然而，shell的本质是调用命令。它并不是一个真正的语言，不能全面的调动计算机的性能。

所以吉多希望有一种语言可以兼具 C 和 shell 的优点。既能全面调用计算机的功能接口，又能轻松的编程。他本来寄希望于ABC语言。ABC语言是由吉多参加设计的一种教学语言(虽然大部分人都没听说过)。从吉多本人的角度来看，ABC这种语言非常的优美和强大(不排除他带了滤镜)，是专门为非程序员设计的。但很遗憾的是ABC语言并没有成功，吉多认为主要原因是这门语言是非开放的。这次的小挫折让吉多决心在这个新的语言中避免这一错误。同时，他还想要实现ABC中没有实现的功能，比如易于传播、可扩展、可以直接进行IO操作等等[1]。

正是因为有这样的念头作为催化剂，吉多才在寒冷的冬夜里，在那些圣诞树上挂着的五颜六色七彩小灯的陪伴下创造了Python！

所以在一门新语言的创造过程中，它的创作者固然居功至伟，但是我们同样也不能否认当时客观的现实条件对语言发展历史也起着巨大的推进作用！

## chapter 2: python的发展

最初的 Python 完全由吉多本人开发。然而此后Guido同事也迅速爱上了这门新语言。他们不断反馈使用意见，并参与到 Python 的改进中。于是吉多和一些同事构成 Python 的核心团队，他们将自己大部分的业余时间用于hack Python（也包括工作时间，因为他们将 Python 用于工作）。

<img src="https://images0.cnblogs.com/blog/92071/201305/06175655-b9ab3a0b656647f0b44ebfdf5f297ae6.jpg" width=150>

由于Python实在是太好用了！很快，Python就拓展到了他们的研究所之外。Python将许多机器层面上的细节隐藏，交给编译器处理，并凸显出逻辑层面的编程思考。这使得程序员可以花更多的时间用于思考程序的逻辑，而不是具体的实现细节。这一特征吸引了广大的程序员。Python开始迅速流行起来。

此外，还有两点外界因素使 Python 得到迅速发展。一是硬件性能的提高，当时已进入90年代初，个人计算机开始进入普通家庭，程序员们开始关注计算机和语言的易用性。相比它的兄弟ABC语言因为硬件的性能限制而失败，Python 可以说是生逢其时，正好有机会可以大展拳脚。二是互联网的发展，当时许多程序员以及资深计算机用户已经开始频繁使用 Internet 进行交流。一种新的软件开发模式开始流行：开源。

开放性是 Python 能够发展壮大的根本原因。吉多是一个很谦逊的人。他自认为自己不是全能型的程序员，所以他只负责制订框架。如果问题太复杂，他会选择绕过去，也就是cut the corner。这些问题最终由社区中的其他人解决。社区中的人才是异常丰富的，就连创建网站，筹集基金这样与开发稍远的事情，也有人乐意于处理。吉多维护了一个 maillist，Python 用户就可以通过邮件进行交流。Python 用户来自许多领域，有不同的背景，对Python也有不同的需求。每当用户不满足于现有功能，很容易对Python进行拓展或改造。随后，这些用户将改动发给 Guido，并由 Guido 决定是否将新的特征加入到 Python 或者标准库中。 而这样的特性不仅减少了开发人员本身的工作量，也使得Python得以快速发展[2]。

所以在Python的后续版本更迭与发展中，Python的创始人吉多在一定程度上很好地处理了他作为创始人与社区之间的关系。吉多扮演了一个被称为一个“仁慈的终生独裁者”的角色，当然，这是一个褒义的委婉说法。如果说的直接一点，那就是吉多本人虽然不参与后续版本更迭代码的编写，但是他一直掌握着将哪些新功能加入Python的最终决定权，换言之他掌握着Python的方向。但是由于吉多谦虚和蔼的个人品质（不同于动辄XXXX的Linux创始人Linus），他可以平衡这巨大的权力与开发者的热情，所以Python的社区关系一直很融洽。但是在2018.7.12，吉多突然宣布放弃了自己仁慈的独裁者的职位，放弃了所有的权力。吉多本人接受采访时说这一方面是由于他考虑退休已经很久了，另一方面，一个颇具争议的Python改进提案（PEP 572）令他受到了大量攻击，最不能忍的是不少攻击来自Python核心成员，这使得他十分心寒。当时这一消息对于Python社区具有爆炸性的效果，出于对吉多的尊敬与爱戴，不少人在祝福的同时都担心Python未来的发展会不会失去方向。但从截至到目前的效果来看，so far so good。

到今天，Python 的框架已经确立。Python 语言以对象为核心组织代码，支持多种编程范式，采用动态类型，自动进行内存回收。Python支持解释运行，并能调用C库进行拓展。由于标准库的体系已经稳定，所以Python的生态系统开始拓展到第三方包。这些包，如Django，web.py，wxpython，numpy，matplotlib，PIL，将 Python 升级成了物种丰富的热带雨林。

如今 Python 已经进入到 3.0 时代，由于 Python 3 向后不兼容，所以从 2.0 到 3.0 的过渡并不容易。而且目前Python的运算性能仍然低于C++和Java，所以在性能方面仍然值得改进。可以说，即使到了今天，Python仍然有着旺盛的生命力，值得我们去用它来创造一个更值得期待的未来[1]。

## chapter 3: python的版本更迭

Python的版本始于1991年。1989年吉多·范罗苏姆开始写Python的解释器。1991，第一个Python解释器诞生。它是用C语言实现的，并能够调用C语言的库文件。这个最初的版本并不具有版本号，但它已经具有了：类，函数，异常处理，包含表和词典在内的核心数据类型，以及模块为基础的拓展系统。

1994年，Python1.0发布，相较于之前的原型，这个正式的版本增加了lambda, map, filter和reduce。之后Python1一直更新到了1.6.1版本，随后被Python2所代替。[4]

2000年，Python2.0发布，加入了内存回收机制，至此奠定了我们现在看到的Python语言的基础。也是从Python2.0开始，Python改变了开发流程，由之前的个人开发转向了社区开发，这使得Python变得更加透明，也带来了活跃的社区与旺盛的生命力。之后，Python2以每一到两年一个版本的速度进行稳定的更新。到了2008年，Python迎来了一次重大的变动——开发组决定开辟一个全新的Python版本，用以彻底解决Python2遗留下来的一堆麻烦。也正是出于这种考虑，Python的这次版本更迭使用了极为罕见的不后向兼容的模式，这就意味这Python2的一些语法与特性不会在新的Python版本中得到支持。于是诞生了Python3，以及困扰了Python社区十年之久的Python2与Python3不兼容问题。

Python3相对于Python2有许多重大改动，包括将Python2中很令人困扰的、作为语句存在的print改为了print函数；将默认支持的编码从ASCII码改成了utf-8；修改了Python2中带有C语言思路痕迹的除法规则与数据类型，整数/整数的结果从只能是整数变成了可以是小数，原来的long类型被删除了，python3只保留int，但它其实就是原来的long；在Python2中一直被大量是用的两种创建迭代器的函数range与xrange被合并了，Python3中只保留了range，但新的range使用的基本上是原来的xrange的机制（这也是为什么Python2与Python3的代码总是存在xrange与range的矛盾）； 删除了原来的不等运算符<>，只保留!=；等等。[5]

但是在2008年Python3发布之后，很多用户的Python2代码因为Python3不支持Python2的问题无法顺利升级到Python3。于是2010年，Python2又发布了一个过渡版本——Python2.7，并一直保持更新。2018年，吉多·范罗苏姆宣布Python2将在2020.1.1到达EOL（end of life 寿终正寝）。这个日期之前的最后一个Python2版本是2.7.17，在它之后到2020.1.1的所有问题，将依然被开发者接受，并在2020年4月的2.7.18中解决，这将是Python2的最后一个版本。[6] 就在本文写作几天前（2020.4.20）Python2.7.18发布，至此，Python2画上了句号。

但Python3仍在茁壮成长。自2008的Python3.0开始，每一到两年更新一个版本，并一直保持小版本的及时更新。Python3的开发者们在这上面也展示出了饱满的热情，每次的版本更新，除了修补发现的问题，还会增加一些新功能（比如3.8的海象运算符）。到本文写作时（2020.4.25），最新的Python3版本是3.8.2，同时3.9正在开发中。

现在，Python具有良好的生态与丰富的第三方库。其中，具有代表性的就是numpy。相信使用过Python的读者多少都使用过或者至少听说过numpy。numpy支持大量的科学计算种类，在底层使用了预编译的C语言代码，所以保证了科学计算的速度。它现在已经基本成为了Python的必备第三方库。如果你想充分利用Python处理大量数据的能力，numpy一定会是一个选项，尤其是在现在人工智能、大数据的浪潮下。它甚至成为了许多其他第三方库的基础，比如最流行的深度学习框架tensorflow与pytorch一定程度上都包含了numpy的核心对象narray。[11] 之所以在这里提到numpy，是因为它的创始人Jim Hugunin与Python有着深厚的缘分，是Python发展历史上的另一个重要人物，不仅仅是因为numpy。我们下面还要详细介绍他。
## chapter 4：IronPython和Jython

说到Python，就不得不提一下在Python的发展过程中延伸出的两个关键分支，Jython和IronPython。

### Jython

Jython和IronPython的故事都要追溯到一个关键的灵魂人物Jim Hugunin，这个人以一己之力对Python
语言作出了无可比拟的贡献，在这里我们先说说他与Jython的故事。

由于Python被开发出来后很快进入了快速发展期，使用Python的人员数目不断增长，然而Sun公司的Java语言也同样深入人心。随着Java实现的项目数量逐渐与C/C++逼近，Python的Java实现也变得很有必要。

Jim Hugunin是吉多在国家研究动力中心(CNRI)的同事，Jython的故事始于他在麻省理工学院完成硕士论文的痛苦。在那篇论文中，吉姆制造、测量和分析了超导体-半导体结，这属于量子计算机的潜在组成部分。为了将分析测量出的结果与理论数据进行比较，他使用了Matlab。但吉姆认为Matlab并不好用，即使拥有出色的数值分析能力，但Matlab并不能进行其他的操作。为了克服Matlab的缺点，吉姆将C、Python和Matlab的代码拼凑到了一起，来计算最终的结果[13]。

但Jim Hugunin知道这并不是解决问题的最佳方案，因此在完成了论文之后，他开始试图像Matlab一样自然地对Python进行扩展以支持数值分析，而又不牺牲Python作为一种丰富的通用编程语言的功能。当他将Numeric Python与其他多种编程语言的性能进行比较时，他惊讶地发现Java对于某些简单的数字基准测试而言，其速度与C语言一样快。

发现了这一点后，Jim Hugunin立刻着手开始实验。他用了一周的时间来试图在Java上使用Python，并且确定了两者之间确实存在着某种优雅而漂亮的匹配。 比如他可以将Python程序手动转换为Java字节码，而不会造成性能上的重大损失。 其次，Java语言与Python有很多相似之处，并且是Python动态特性的静态替代品。 最后，他发现了一个很棒的java.reflect包，该包使得使用者无需其他额外操作就可以从Python加载和使用任意Java库。 这意味着我们应该可以从网上下载一个有趣的新Java库，将其放在类路径中，然后立即从Python开始使用它。

Jim Hugunin实现了最初版本的Jython，但后续由于要开发aspectj，Jython的开发由其他人接手。Python和Jython项目组从CNRI离开后，在Sourceforge上转变为一种更开放的语言模型。由于兼具了Java和Python的特点，Jython既可以对Java类做到无缝存取，又同时具有Python简明、方便和易读的特性。Jython使用缩排来对代码块定界以避免使用在Java中的大括号，并用新的一行来表示一个新的语句的开始，而且允许在语句后省略分号。Jython没有像在Java中的public、private和protected存取符，这样就给程序员提供了快速开发所需要的灵活性，并将注意力集中在程序逻辑上。正像前面所提到的，Jython不用明显的静态的类型定义，故程序员不需要从程序逻辑转移到类型定义上来。

Jython最初的含义是Python on JVM，所以最初的名称是JPython，后续由于基于JVM可以有更多可能性，名字改为Jython。Jython的版本开发暂停于2.7.2，除了Python社区比较分散，在 Java 生态圈得不到足够强大的支持，发展不起来的原因之外，与它的主要作者吉姆被微软雇用去开发IronPython想必也有很大的关系[12]。

### IronPython

IronPython其实就是一个C#版本的Python解释器，是一种在 NET 和 Mono 上实现的 Python 语言，还是由Jim Hugunin创造，使用动态类型系统将Python移植到了NET Framework上。

当初，Jim Hugunin通过阅读网上的无数CLR(common language runtime)报告了解到，对于动态语言尤其是Python来说，CLR是一个极其糟糕的平台。按照他的话说：“最初的IronPython是作为一系列快速原型而面世的，创建它的初衷只是用来帮我了解这个平台到底有多么糟糕。我的计划是编写一个简练的论文，名称为“为什么CLR是一个糟糕透顶的动态语言平台”。后来，这些原型这个竟然运行百的很好，通常它们比基于标准C的Python实现要快多了，所以原来的计划也由此被打乱了。”

在构造IronPython的过程中，Jim Hugunin和CLR团队进行了深入的交流。最终，他决定加入微软，加入CLR团队，这个时候Jim Hugunin并不是IronPython的开发者了，他们开始构造更适合动态语言的CLR。DLR（Dynamic Language Runtime）就是他们的工作成果之一。

DLR构建在CLR之上，提供了一批服务和API，使得语言开发者能够容易地构造编程语言。它不但是IronPython 2.x的基础，也是C# 4.0的基础。C# 4.0提供了dynamic关键字，可以实现运行时的结构一致性语义（即duck typing）。从语句表达，到底层实现，C#已经完全动态化，动态语义已经渗入其机理。可见，DLR不但打通了IronPython与C#交互的关键，也必将影响到.NET平台上的所有开发者。

IronPython与DLR是共生关系：CLR团队用IronPython来驱动DLR的开发，DLR的开发成果又反过来支持IronPython的进一步演化。这也表明，IronPython将受到微软的持续支持。也许有人会问：既然C# 4.0已经动态化，那么为什么还需要掌握一种“真正”的动态语言呢？Harry Pierson的回答是：用合适的工具做事（choose the right tool for the job）。Harry曾经是C#最早一批的开发者和使用者，后来曾任IronPython团队的程序经理。与《IronPython in Action》的作者Michael Foord相似，他很擅长也很喜欢C#，同时也非常热爱IronPython。

IronPython的1.0版本在2006年被发布。这个版本具有很大的技术漏洞，比如它创建的所有动态生成的代码永远都不会被垃圾回收，从而导致巨大的内存泄漏。同时，它使用微软单方面的“开源”协议（译注：即MS-PL），但没有得到社区的信任。在接下里的几年里这个协议通过了OSI认证，最后IronPython转向了更著名的Apache开源协议。2008 年，随着微软发布 NET Framework3.0/3.5、Silverlight 之后，IronPython也发布了 2.0 版。

2010年10月，在Microsoft中止了对IronPython的投资，这也成为了Jim Hugunin离开微软加入谷歌的导火索。接下来的几年，频繁更换组织者的IronPython项目的发展无比缓慢，最新版本于2020年4月27日发布，已经可以提供.NET Core和.NET Standard支持。

将来IronPython可能会是一个成功的项目，因为IronPython没有全局解释器锁。很多Python实现都有这个特性，这也是高性能的绊脚石。所以我们依然期待着IronPython可以实现长久以来快速、多核友好的Python的梦想[14]。


## chapter 5：Jim Hugunin
IronPython是一个与.NET框架紧密集成的Python编程语言的一个开源实现。IronPython能够使用.NET框架和Python库，并且其他.NET语言可以很容易的使用Python代码。IronPython是.NET框架的一个优秀补充，为Python开发人员提供了.NET框架的强大功能。现有的.NET开发人员也可以使用IronPython作为一种快速且富有表现力的脚本语言，用于嵌入、测试或从头开始编写新的应用程序[7]。  

IronPython是在动态语言运行时(DLR)之上实现的，DLR是一个运行在公共语言基础结构之上的库，它为动态语言提供动态类型和动态方法分派等功能。

IronPython完全是用c#编写的，尽管它的一些代码是由用Python编写的代码生成器自动生成的。

吉姆（Jim Hugunin）创建了这个项目，并且直到2006年9月5日发布的1.0版本，他都一直积极参与其中[8]。  
![Jim Hugunin headshot](https://github.com/BIT-SYS/Open-source-stories/raw/master/img/Jim_hugunin_headshot.jpg)  

2010年，微软放弃对IronPython的投资，吉姆离开微软加入了谷歌。在吉姆的个人网站中，他表示“将微软对于IronPython的决定是我离开微软的催化剂，但不能算是原因”。他还表示，在微软有一个“开源代码和社区保持健康的关系”是“可能的”，但“感觉就像把方钉入圆孔”[9]。  

最后，Jim表示他将退出IronPython项目。目前IronPython已经有了新的组织者，他们是Miguel de Icaza、Michael Foord、Jeff Hardy与Jimmy Schementi，其中Miguel de Icaza和Jimmy Schement同时也会负责IronRuby项目的协调工作[10]。

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
[10]https://www.cr173.com/html/7617_1.html  
[11]https://www.numpy.org.cn/user/setting-up.html  
[12]https://www.jython.org
[13]http://hugunin.net
[14]https://ironpython.net
