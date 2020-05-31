# 苹果的太子——Swift

## chapter0 诞生

与我们在这里介绍的其他大多数语言都不同，Swift语言并不是由一个或几个天才凑到一起鼓捣出来的语言。从一开始，它的背后就站立着一个巨人的身影——苹果公司。所以Swift的开源故事并不像之前的故事一样，充满了天才与极客的光环；相反，它包含着浓浓的商业气息。Swift语言本身也像iPad、iPhone或其他的苹果产品一样，针对的是一个苹果公司所指定的范围，并且在这个范围之内表现良好。不论现在Swift现在都有哪些应用，在它诞生之初，苹果公司给它的使命就是专门针对OS X和iOS的应用开发；不论Swift以后又可能被应用到什么地方，它最核心的功能始终都是苹果设备上的应用开发。所以某种程度上说，Swift是苹果的嫡系，一荣俱荣，一损俱损。

因为Swift是苹果公司推出的，所以它是现代软件工程团队合作的结果，我们很难给他找出一位或者几位创始人。相应地，在人物这一环节我们关注的将是苹果公司。

Swift的诞生应当算是2014年。在2014年的苹果开发者大会（WWDC）上，时任苹果公司CEO蒂姆库克发布了iOS 8，与之同时发布的就是Swift。Swift独立于C语言与苹果之前使用的Objective-C，苹果希望Swift可以为其旗下产品带来更好的体验。但既然是苹果公司为自身产品定做的语言，自然要考虑兼容的问题，这款新的语言应当可以与之前苹果系统内软件开发所用语言兼容，具体来讲，就是Swift应该与Objective-C兼容。而苹果也的确考虑了这一点。Swift使用了Objective-C的命名参数以及动态对象模型，可以无缝对接到现有的Cocoa框架，并且可以兼容Objective-C代码。但它在各个方面优于 Objective-C，也不会有那么多复杂的符号和表达式。可以说，Swift是基于Objective-C的改进，它在编程语言上的父亲是Objective-C语言。

## chapter1 Objective-C与苹果

我们在这里就有必要介绍以下Objective-C在苹果公司的历史，尤其是这中间还包含了史蒂夫·乔布斯（Steve Jobs）与他的苹果公司的往日恩怨。

Objective-C是在1980年代初由布莱德·考克斯(Brad Cox)在他自己的公司Stepstone创建的。考克斯当时想打造的是一门流行的、可移植的C语言与优雅的Smalltalk的结合体，于是在C的基础上，加入面向对象特性就得到了Objective-C，这从它的名字也可以看出来（对象的C）。考克斯本人的专业领域是软件工程，所以Objective-C的核心思想是软件重用性，组建化。

Objective-C与苹果产生联系是1985年之后的事，这一年，史蒂夫·乔布斯引狼入室。他之前从百事可乐挖来苹果担任CEO的约翰·斯卡利（John Sculley）与董事会将他赶出了他一手创立的苹果公司。被扫地出门后，乔布斯创建了NeXT电脑公司，并发展出NeXT电脑与NeXT STEP操作系统。正是在NeXT STEP操作系统上，Objective-C语言得到了应用。NeXT公司从Stepstone公司获得了Objective-C的授权，并且可以开发自己的Objective-C编译器与库。基于Objective-C，NeXT开发了它们的NeXT STEP操作系统，并创建了用于开发用户界面的NeXTSTEP Toolkit软件包。

这里插一句题外话，第一台万维网服务器正是蒂姆·伯纳斯·李在NeXT STEP上写的，这其中自然也有Objective-C的功劳。

1993，NeXT公司放弃了硬件业务，专注于软件，也就是他们的NeXT STEP操作系统上。他们与太阳公司（SUN）一起搞出来了一个NeXT STEP的升级版OPENSTEP，它可以运行在Soloris和Windows NT。

1995年，NeXT从考克斯的Stepstone公司拿到了Objective-C。到这里，似乎Objective-C都和苹果没什么关系。但别着急。

1996年，苹果买下了它的创始人被扫地出门后创建的NeXT公司，其主要目的就是用NeXT的NeXT STEP操作系统取代老旧的Mac OS。伴随着收购，乔布斯重回苹果董事会。

1997年，乔布斯以救世主的姿态重新出任苹果CEO。

伴随着NeXT STEP进入苹果的操作系统与乔布斯成为CEO，OBjective—C语言也进入了苹果的技术栈。这其中一方面是由于新的Mac OS基于NeXT STEP，就必然要引入Objective-C；另一方面可能是因为乔布斯个人，他著名的控制欲使他一直想要掌握他产品的各个方面，包括编程语言在内，所以使用完全在自己手里的Objective-C就是很好的选择。从2001年苹果发布的Mac OS X开始，Objective-C，以及NeXTStep和OpenStep所引入的面向对象技术就在苹果公司的产品中大量使用了。后来，Objective-C被用来在XCode IDE下编写本地面向对象的“Cocoa”API，这些API是iOS上手势识别和动画功能的核心，这些功能为iPhone和iPad增光不少。Objective-C还提供了Foundation Kit和Application Kit，用于构建本地的OS X和iOS应用程序。

## chapter2 Swift的发展

但是随着时代的发展，Objective-C变得越来越不方便了。从某种程度上说，它太古老而特殊了。开发者必须使用专有编程系统，这使得开发者很难写出高质量的跨平台软件，因此必须投资大量精力在OSX/iOS平台上，从而无暇顾及和Apple竞争的平台。这甚至引起了开发者相当程度的不满。作为应对，苹果顺势推出了Swift作为替代。Swift可以完全兼容Objective-C，它取代了Objective-C成为苹果生态圈内的编程语言。

2010年，LLVM编译器的原作者，同时也是苹果开发者工具部门总监克里斯·拉特纳（Chris Lattner）开始着手创建Swift编程语言的工作，还有一个团队大力参与其中。拉特纳主要负责了Swift的架构，如果要给Swift找出来一个作者，那么拉特纳是比较合适的。经历了四年的时间，2014年的苹果开发者大会上，Swift发布。

2014年6月，就在苹果开发者大会后不久，《Swift中文版》发布。

2015年年12月4日，苹果公司在苹果开发者大会上宣布将将Swift开源。长达600多页的《The Swift Programming Language》可以在线免费下载。

2015年6月，Swift发布了2.0版。

2016年9月，Swift发布了3.0版。

2017年9月，Swift发布了4.0版。

2019年，Swift发布5.0版。这也是目前（截至2020年5月的最新版本）。到此为止，Swift的ABI（Application Binary Interface 应用程序二进制接口）终于稳定。目前Swift可以在所有苹果平台与Linux平台上运行。




## chapter3 Swift的特点

### 与Objective—C相比

与Objective-C相比，Swift取消了预编译指令，宏也被包括在内；取消了Objective-C中的指针等其他不安全访问的使用；在swift中不再有.h和.m文件之分的。所有的代码全部都存储在一个文件里面；Swift中所有的代码都被封装在{}里面；Swift使用()取代了Objective-C中进行初始化的alloc init；OC中使用[]来调用方法，而Swift中采用点语法；Swift不使用分号分隔语句。

### 编译特点

由于Swift是苹果公司出品，它的编译也打上了苹果的烙印。我们都知道拉特纳2005进入苹果后。就职于苹果公司并领导一个专门为苹果开发系统研发编译器的工作组，该工作组基于 LLVM 支持苹果各类系统研发，并使 LLVM 成为苹果 macOS 和 iOS开发工具的一部分。因此LLVM是苹果一直使用的编译器，最开始，LLVM打算使用GCC作为前端，后来为了改善对Objective-C的支持并避免开源协议的纠纷，苹果开发了一个基于LLVM的新编译器前端，就是Clang。到了Swift，苹果沿用了LLVM编译器后端，用一个叫swiftc的编译器前端代替了clang。

### 易上手

大多数用过Swift的人都承认这款语言对于初学者还是很友好的。苹果设计这款语言的初中跟他们设计iPhone、iPad的理念是相同的，即希望对用户友好、使得任何人都能使用。Swift中很多现代化的设计实现了这一点，比如泛型、元组和多值返回、对范围或集合进行快速迭代等等。并且苹果还在他们的APP store中提供了面型首次学习编程初学者的APP，以及面向有经验开发者的免费课程。

### 安全性

尽管苹声称Swift具有良好的安全性，但这些年来Swift在安全性上的表现并不是很好。根据Veracode发布的年度软件安全现状报告，Swift代码库的软件缺陷密度已经超过了PHP。在该报告中Swift以7个位居bug密度榜首，不过在可利用的PoC上，Swift的表现不算糟，跟Python持平，还少于Java。

## Reference

[1]https://www.jianshu.com/p/26bac82ab683

[2]https://baike.baidu.com/item/SWIFT/14080957?fr=aladdin

[3]https://developer.apple.com/cn/swift/

[4]https://blog.csdn.net/weixin_42433480/article/details/92669163
