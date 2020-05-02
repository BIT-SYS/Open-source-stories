# 并非派生于Java的JavaScript

## chapter 0：JavaScript的诞生
相信不少朋友第一次听到JavaScript时会觉得它和Java有某种冥冥之中的联系，会猜想JavaScript是不是Java的脚本语言？但事实上，尽管JavaScript和Java之间有相似之处，包括语言名称、语法和各自的标准库，但这两种语言在设计上是截然不同的。JavaScript语言最初出现在Netscape Navigator 2浏览器中。当时它叫LiveScript。然而，由于当时Java技术如日中天，网景（Netscape）公司觉得改为JavaScript这个名字会更吸引人注目[1]。  

JavaScript,通常缩写为JS，是一种符合ECMAScript规范的编程语言。  

1994年，网景公司发布了Navigator浏览器0.9版。这是历史上第一个比较成熟的网络浏览器，轰动一时。但是，这个版本的浏览器只能用来浏览，不具备与访问者互动的能力。网景公司急需一种网页脚本语言，使得浏览器可以与网页互动。  
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/Navigator%E6%B5%8F%E8%A7%88%E5%99%A8.png" width="320">
</div>
当时，开发新的网页脚本语言有两种方式选择，一是将现有语言嵌入到网页中，如Perl、Python、Tcl、Scheme等等，二是开发一个全新的语言，网景公司管理层对此争执不下。就在这时，发生了另外一件大事：1995年Sun公司将Oak语言改名为Java，正式向市场推出。Sun公司大肆宣传，许诺这种语言可以"一次编写，到处运行"（Write Once, Run Anywhere），它看上去很可能成为未来的主宰。于是，当时的形势就是，网景公司的整个管理层，都是Java的信徒，Sun公司完全介入网页脚本语言的决策。  

这时，34岁的系统程序员Brendan Eich登场了。1995年4月，网景公司录用了他。网景公司录用布兰登的目的是研究将Scheme语言作为网页脚本语言的可能性，布兰登本人也认为自己进入公司后将主要与Scheme打交道。但仅仅一个月后，也就是1995年5月，网景公司做出决策，未来的网页脚本语言必须"看上去与Java足够相似"，但是比Java简单，能够让非专业的网页作者也可以很快上手。这就将Perl、Python、Tcl、Scheme等非面向对象编程的语言排除在外了。而布兰登，被指定为这种"简化版Java语言"的设计师。  
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/Brendan_Eich.jpg" width="160">
</div>

然而，布兰登本人对Java并不感兴趣，但为了应付公司的任务，他还是将其设计出来了（仅用了10天！），最初命名为LiveScript，之后改为JavaScript，并对外宣称JavaScript是Java的补充。但也因为设计时间短，JavaScript有很多不完善的地方，这导致之后很长一段时间，JavaScript写出来的程序混乱不堪。如果当时布兰登意识到JavaScript将会被数以百万计的人员学习和使用，不知道会不会在它上面多花心思呢？  

布兰登设计JavaScript的思路可以概括如下：  
- 借鉴C语言的基本语法  
- 借鉴Java语言的数据类型和内存管理  
- 借鉴Scheme语言，将函数提升到"第一等公民"（first class）的地位  
- 借鉴Self语言，使用基于原型（prototype）的继承机制  

事实上，布兰登本人一点也不喜欢自己的这个作品。"与其说我爱Javascript，不如说我恨它。它是C语言和Self语言一夜情的产物。十八世纪英国文学家约翰逊博士说得好：'它的优秀之处并非原创，它的原创之处并不优秀。'（the part that is good is not original, and the part that is original is not good.）"[2]。  

## chapter 1：JavaScript和Java的关系与区别
如果非要说JavaScript和Java之间有什么关系，那可能是雷锋和雷峰塔的关系[3]。  

首先，上面提到，JavaScript借鉴了Java语言的数据类型和内存管理

JavaScript 语言的函数是一种独立的数据类型，以及采用基于原型对象（prototype）的继承链。这是它与Java语法最大的两点区别。JavaScript 语法要比 Java 自由得多。  

另外，Java需要编译，而JavaScript则是运行时由解释器直接执行。  

总之，JavaScript的原始设计目标是一种小型的、简单的动态语言（10天大概也设计不出来复杂的东西），与 Java 有足够的相似性，使得使用者（尤其是Java程序员）可以快速上手[4]。  

## chapter 2：JavaScript的发展
### 浏览器大战中的JavaScript
浏览器是一个苛刻的环境，以发展为目标，不仅互联网采用率低，互联网连接缓慢，而且浏览器大战（主要是在网景和微软之间）引发了很多混乱。  

Netscape Navigator 4于1997年发布，Internet Explorer 5于1998年发布。  

与其他语言相比，JavaScript非常不同。它没有编译器，没有调试器（至少不是很好的调试器），没有办法“运行JavaScript程序”，除了在浏览器中编写脚本，并查看它们是否运行。 JavaScript的开发工具仍然是原始的或不存在的。并且JS没有太多的开源社区，要弄清楚如何实现某项功能，通常会在其他人的网站上“查看源码”。 此外，Web开发人员编程社区中的大部分讨论都是JavaScript中兼容性和安全性的噩梦。  

### 2008年的JavaScript
大约在这个时候，一些JavaScript库变得流行，特别是jQuery，Prototype，YUI和Dojo。 这些库试图为JavaScript提供它缺少的东西：跨浏览器兼容性和编程模型，用于对浏览器内的页面进行动态操作，特别是对于新出现的JavaScript编程模型AJAX。 这是“动态”Web应用程序，单页应用程序等趋势的开始。  

### JavaScript工具集的飞跃
JavaScript的开发工具也取得了一些重要的飞跃。 2006年，Firefox团队发布了Firebug，这是Firefox的JavaScript和DOM调试器，后来Firefox成为世界上最受欢迎的Web浏览器之一，也是开源的。两年后，谷歌将首次发布谷歌Chrome，它捆绑了一些开发人员工具。大约在Chrome发布的同时，谷歌还发布了V8，这是嵌入Chrome内部的JavaScript引擎。这标志着世界第一次看到JavaScript语言的完整，高性能的开源实现，并没有完全与浏览器绑定。 Firefox的JS引擎SpiderMonkey是其源代码树的一部分，但不一定是在Firefox浏览器的上下文之外进行模块化和使用[5]。  

## chapter 3：JavaScript与ECMA的关系
1996年，微软模仿JavaScript开发了一门相近的语言JScript，内置于IE3.0，Netscape公司面临丧失浏览器脚本语言的主导权局面。胳膊拗不过大腿，Netscape又找了个大哥-国际标准化组织ECMA（European Computer Manufacture Association）来抵抗微软。  

​1997年，ECMA组织发布262号标准文件（ECMA-262），里面规定了浏览器脚本语言的标准，并将这种语言成为ECMAScript[7]。  

## chapter 4：JavaScript版本迭代
文章上面标准化部分提到，JavaScript于1997年成为ECMA标准，而ECMAScript就是该语言的官方名称。  

从1997年的ECMAScript 1到2009年的ECMAScript 5（其中	ECMAScript 4从未发布），其依次做以下几点变更：改变编辑方式；添加正则表达式与try/catch语句；添加“严格模式”、JSON支持、String.trim()、Arrary.isArrary()和数组迭代方法。  

2001年，推出了命名为ECMAScript 5.1的版本，主要做了编辑的改变。  

2015年到2018年，以一年一次的频率发布了ECMAScript 2015到ECMAScript 2018版本。ECMAScript 2015添加了let、const、默认参数值、Arrary.find()、Arrary.findIndex()。ECMAScript 2016添加了指数运算符（**）和Array.prototype.includes。ECMAScript 2017添加了字符串填充、新的Object属性、异步功能以及共享内存。ECMAScript 2018添加了rest/spread 属性、异步迭代、Promise.finally()以及RegExp[6]。  

## chapter 5：有关布兰登的一些趣闻
布兰登的技术很牛，眼界宽广，表达能力也非常强，因此在网景公司内部他的话很有影响力。与他共事的工程师，在互联网上与他交流的开发者，甚至包括他遇见的高管们都非常赞赏他，赞赏他过人的才华、谦逊的态度和热心肠。  

布兰登呆在电脑前就是一个恶魔，从舍不得浪费半点时间。如果同事因为某个问题打断了他与他交谈时，往往的结果就是，他会继续编程，收邮件，或者干脆同时与别人聊天，留给同事的只有半个侧脸。当谈话者要求他专心点，他就说他很忙，需要回去工作了。  

布兰登在空闲时，会演奏古典钢琴或者体操。他还喜欢旅行，当然他更喜欢工作！——他很多假期都被填满了，因为他有很多预先打算的事情要做[8]。



## Reference
[1]https://blog.csdn.net/lewis_lyx/article/details/7375330?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-2&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-2  
[2]https://blog.csdn.net/kese7952/article/details/79357868  
[3]https://www.zhihu.com/question/19913979  
[4]https://www.jianshu.com/p/80e789c670aa  
[5]https://www.cnblogs.com/wdsunny/p/11428307.html  
[6]https://zixuephp.net/manual-javascript-691.html  
[7]https://www.cnblogs.com/wenha/p/12079168.html  
[8]https://zhuanlan.zhihu.com/p/19778958


