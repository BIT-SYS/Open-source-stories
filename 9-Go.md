# 易用与高效的结合——Go语言

## chapter 0：Go语言的诞生
Go语言（又称Golang）由三位Google的员工罗伯特·格瑞史莫（Robert Griesemer）、罗勃·派克（Rob Pike）以及肯·汤普逊（Ken Thompson）共同设计而成[1]，当时他们正遭受C++这种复杂难用的语言的折磨，所以在设计Go语言之初有一个明确的目标——设计一种易于使用的语言，同时它仍能应对公司错综复杂的系统带来的挑战。派克曾提到“Go项目的目标是消除在谷歌上软件开发的缓慢和笨拙，从而使过程更有生产力和可伸缩性。Go语言是由写、读、调试和维护大型软件系统的人员设计的。”[2]  

说到Go的诞生，不得不提的是Google著名的‘20% time’政策。Google鼓励员工，除了他们的常规项目外，花20%的时间在他们认为最有利于谷歌的项目上，这使员工更有创造力和创新性。Google的许多重大进展都是以这种方式取得的，当然，包括最初的Go语言[6]。

可能是Go语言的诞生减轻了其他复杂语言带来的许多烦恼，它被给予了一个非常可爱的吉祥物——Go地鼠。Go地鼠有自己独一无二的特性，就像高飞不是一只老卡通狗（布鲁托）一样，它也不是一只老地鼠[3]。由于可爱的外表，Go地鼠甚至还出了周边......
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/gopher.png" width="120">
</div>  

Go经常被称为Golang，主要是因为其网站域名golang.org（在美国go.org是不被允许的），但无论如何它只有一个真正的名字——Go[4]。

## chapter 1：Go语言创始人  
前面已经提到，Go语言最初的创始人有格瑞史莫、派克和汤普逊，他们都是Google的员工。 
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/authorOfGo.png" width="200">
</div>  
###派克
派克最出名的是在Go编程语言和贝尔实验室的工作，他是Unix团队的一员，参与了贝尔实验室和Inferno操作系统的Plan 9，以及Limbo编程语言的创建。他与汤普逊共事多年，并共创出广泛使用的UTF-8字元编码。
###汤普逊
汤普逊职业生涯的大部分时间都在贝尔实验室工作，在那里他设计并实现了最初的Unix操作系统。他还发明了B语言，C语言的直接前身，也是Plan 9操作系统的创造者和早期开发者之一。自2006年以来，汤普森一直在Google工作，并在Google参与了Go语言的研发工作[7]。
###格瑞史莫
在开发Go之前是Google V8、Chubby和HotSpot JVM的主要贡献者[6]。
## chapter 2：Go语言特性
Go语言保证了既能达到静态编译语言的安全和性能，又能达到动态语言开发维护的高效率，使用一个表达式来形容Go语言：Go=C+Python，也就是说，Go试图将动态语言(如Python)的简单易用与编译语言(如C或c++)的性能和安全性结合起来。[5]。Go语言一些主要特色如下：
### 受C语言影响
为了使Go语言能够提供较高的效率，其从C语言继承了许多理念，包括表达式语法、控制结构、基础数据类型、调用参数传值等等，也保留了和C语言一样的编译执行方式及弱化的指针。
### 内置并发机制  
Go包括运行并发任务的内置机制。使用称为“goroutines”的轻量级进程，使用者可以轻松地在同一个操作系统线程中切换多个任务，或者将它们分散到不同的线程中，所有这些都是由Go运行时自动调度的。  

同时，Go语言实现了CSP（通信顺序进程，Communicating Sequential Process）模型来作为goroutine间的推荐通信方式，在CSP模型中，一个并发系统由若干并行运行的顺序进程组成，每个进程不能对其他进程的变量赋值。进程之间只能通过一对通信原语实现协作。Go语言用channel（通道）这个概念来轻巧地实现了CSP模型。channel的使用方式比较接近Unix系统中的管道（pipe）概念，可以方便地进行跨goroutine的通信[5]。
###垃圾回收机制
Go将内存使用保持在最低限度。它提供了垃圾收集，但也让使用者免于线程过载。“我们不必担心我们正在运行的线程数量。我们不是一直在问‘我们的资源是否已经耗尽了?’”Rarick解释道，“我们可以用很多goroutines来代替，这是语言中内置的。”  


这是一个独特的组合。C提供了控制权，但它并不适合并发。它甚至不给你进行垃圾收集。Go提供了并发性和垃圾收集，但它仍然为您提供了对内存布局和资源使用的控制。  
##chapter 3：Go语言发展历史
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/GoHistory.png" width="250">
</div>  

自最初发布以来，Golang发生了很大的变化，包括语法和语义等。谷歌试图从语言中去除C的痕迹，从而使其结构更易于使用和自给自足。于是，Golang对以前没有其他编程语言经验的开发人员变得更加友好。  

从版本1.0至今，Go最新的发行版本已经到了1.14。
<div align=center>
	<img src="https://github.com/BIT-SYS/Open-source-stories/raw/master/img/go_versions.jpg" width="250">
</div>  


## Reference
[1]https://en.wikipedia.org/wiki/Go_(programming_language)  
[2]https://qarea.com/blog/the-evolution-of-go-a-history-of-success  
[3]https://blog.golang.org/gopher  
[4]https://golang.org/doc/faq#go_or_golang  
[5]https://studygolang.com/articles/26669  
[6]https://juejin.im/post/5c9b2da26fb9a070cf6be107  
[7]https://en.wikipedia.org/wiki/Ken_Thompson  
