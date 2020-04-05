### 编译器
#### GCC C
GNU编译器套装（英语：GNU Compiler Collection，缩写为GCC），指一套编程语言编译器，以GPL及LGPL许可证所发行的自由软件，也是GNU计划的关键部分，也是GNU工具链的主要组成部分之一。GCC（特别是其中的C语言编译器）也常被认为是跨平台编译器的事实标准。1985年由理查德·马修·斯托曼开始发展，现在由自由软件基金会负责维护工作。

原名为GNU C语言编译器（GNU C Compiler），因为它原本只能处理C语言。GCC在发布后很快地得到扩展，变得可处理C++。之后也变得可处理Fortran、Pascal、Objective-C、Java、Ada，Go与其他语言。

许多操作系统，包括许多类Unix系统，如Linux及BSD家族都采用GCC作为标准编译器。

GCC原本用C开发，后来因为LLVM、Clang的崛起，它更快地将开发语言转换为C++。许多C的爱好者在对C++一知半解的情况下主观认定C++的性能一定会输给C，但是Ian Lance Taylor给出了不同的意见，并表明C++不但性能不输给C，而且能设计出更好，更容易维护的程序[11]。
#### Clang
是一个C、C++、Objective-C和Objective-C++编程语言的编译器前端。它采用了LLVM作为其后端，而且由LLVM2.6开始，一起发布新版本。它的目标是提供一个GNU编译器套装（GCC）的替代品，支持了GNU编译器大多数的编译设置以及非官方语言的扩展。作者是克里斯·拉特纳（Chris Lattner），在苹果公司的赞助支持下进行开发，而源代码许可是使用类BSD的伊利诺伊大学厄巴纳-香槟分校开源码许可。Clang项目包括Clang前端和Clang静态分析器等[12]。
#### Small-c
Small-c既是C编程语言的一个子集，适用于资源有限的微型计算机和嵌入式系统，也是该子集的一个实现。最初作为1970年代末和1980年代初可用的微型计算机系统的早期编译器是很有价值的，作为一个简单到足以用于教学目的的例子，这个实现也很有用。  

最初的编译器是Ron Cain用Small-C为Intel 8080编写的，发表在1980年5月的*Dr. Dobb's Journal of Computer Calisthenics & Orthodontia*上。James E. Hendrix改进并扩展了最初的编译器，并编写了Small-c手册。Ron使用John Bass提供的Small-c开发的账号在SRI PDP 11/45 Unix系统上启动了Small-c。提供的源代码是在管理权限下发布到公共域的。Small-c对于微型计算机非常重要，这在某种程度上类似于GCC对于大型计算机的重要性

Small-c是一个可重定向编译器。移植Small-c只需要为目标处理器重写后端代码生成器和库到操作系统接口调用。[13]
#### Intel C++ Compiler
Intel C++ Compiler，也称为icc或icl，是一组来自Intel的C和C++编译器，适用于Windows、Mac、Linux、FreeBSD和基于Intel的Android设备[14]。  

### C语言库
#### libc
如ANSI C标准中所述，C标准库libc是C编程语言的标准库。它是与C库POSIX规范同时开发的，后者是它的超集。由于ANSI C被国际标准化组织采用，C标准库也被称为ISO C库。  
C标准库为诸如字符串处理、数学计算、输入/输出处理、内存管理和其他操作系统服务等任务提供宏、类型定义和函数[15]。
#### glibc
glibc(GNU C Library)项目为GNU系统、GNU/Linux系统,以及许多其他使用Linux作为内核的系统提供了核心库。这些库提供了关键的API，包括ISO C11、POSIX.1-2008、BSD、针对于操作系统的API等等。这些API包括诸如open、read、write、malloc、printf、getaddrinfo、dlopen、pthread_create、crypt、login、exit等。  
GNU C库被设计成一个向后兼容的、可移植的、高性能的ISO C库。它旨在遵循所有相关标准，包括ISO C11、POSIX.1-2008和IEEE 754-2008[16]。
#### glib
GLib是一个跨平台的、用C语言编写的五个底层库的集合，为GNOME所使用。GLib起初是GTK+的一部分，但到了GTK+第二版，开发者决定把跟图形界面无关的代码分开，这些代码于是就组装成了GLib。  
因为GLib具有跨平台特性，所以用它编写的程序可以无需进行大幅度修改就可以在其他程序上编译和运行[17]。


[11]https://zh.wikipedia.org/wiki/GNU_Compiler_Collection  

[12]https://zh.wikipedia.org/wiki/Clang  

[13]https://en.wikipedia.org/wiki/Small-C  

[14]https://en.wikipedia.org/wiki/Intel_C%2B%2B_Compiler  

[15]https://en.wikipedia.org/wiki/C_standard_library 
 
[16]https://www.gnu.org/software/libc/  

[17]https://zh.wikipedia.org/wiki/GLib  

