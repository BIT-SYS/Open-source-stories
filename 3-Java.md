# Java与OpenJDK的前世今生

## Java的诞生
 
1991年，Sun Microsystems公司的James Gosling和他的项目组（Green Team）启动了一个名为“Oak”的项目，这个项目的目标是实现一个虚拟机并设计一个与C类似但比C/C++简单的语言，最初是为了用于可交互电视的嵌入式应用。由于Oak商标已经被占用，所以改名为Java，并于1995年发布了1.0版本。在讨论名字的时候，项目组成员提出了许多候选项，Java是印度尼西亚的一个岛屿，那里出产了第一种咖啡（称为java coffee），是一种浓缩咖啡豆。James Gosling在办公室附近喝咖啡时选定了Java这个名字[3]。

图 1 Green Team合影 [4]

由于其虚拟机免费，支持大多数主流平台，安全且可配置，并做到了“Write Once， Run Anywhere”的承诺，很快得到了Netscape、Oracle和Microsoft等公司的支持。随后发布的Java 2中包括了J2EE和J2SE，分别对应企业版和标准版。Sun一直没有对Java标准版收费，但是在企业版取得了相应的回报。Sun公司将JDK（Software Development Kit）和JRE（Runtime Environment）分开，二者的区别主要在于，JRE中并没有包含Java编译器。

## OpenJDK的曲折之路
之后Java一直平稳发展[4]，直到2006年在Javaone大会上，Sun公司宣布会将Java开源，同年10月再Oracle OpenWorld会议上，Jonathan Schwartz称Java核心平台将在30天到60天内开源。2006年12月，Sun终于将Java HotSpot虚拟机和编译器开源，并使用了GNU GPL协议，并承诺除了个别组件外，JDK的其他部分（主要是Java运行时）将于2007年3月同样按照GPL协议开源，少数组件不能开源主要是因为Sun没有权限将这些构件以GPL的形式开源。按照开源鼻祖Richard Stallman的说法，这将终止Java的开源之路[2]。
遵照之前的承诺，2007年上半年Sun公司以GPL发布了Java Class Library的绝大部分代码，其中一些受限的部分是由第三方授权给Sun公司的，而Sun不能修改开源协议以GPL协议开源，其中就包括了Java图形用户接口GUI。Sun声称他们计划用其他实现替换这些专属模块，以实现类库的完全开源。
2007年5月发布的时候，OpenJDK的类库中有4%是没有开源的，到2008年5月OpenJDK 6出现的时候，只有不到1%的部分没有开源，但是这1%涉及的部分（SNMP）并没有在Java规范中，因此基本上不需要其他的任何的二进制插件就可以构建出OpenJDK。阻碍开源的每个组件要不自己变成了免费的开源软件，要不就被替换掉了。2010年12月，JDK终于实现了完全开源，这也是Sun Microsystems和OpenJDK社区长期共同努力的结果。

## Java的版本号之谜

1998年，Sun公司发布了第二代Java平台的3个版本，J2ME，J2SE和J2EE，分别代表Java2 Micro Edition、Java 2 Standard Edition、Java 2Enterprise Edition，JDK从1995年到2002年J2SE 1.4发布都按照1.x的格式命名，但是从2004年开始，J2SE的版本变为了5.0，也就是将1.5.0前面的“1.0”去掉了，这主要是为了反映该版本的重要性，即J2SE的成熟度、稳定性、可伸缩性和安全性都有了较大的提升。虽然产品的版本号变成了5.0，但是内部的开发版本号仍然沿袭了以前的习惯使用1.5.0。从2006年开始发布的新版本中，将J2SE中的“2”去掉，命名为Java SE 6。2017年9月，Java平台的首席架构师Mark Reinhold建议将每两年发布一次改为每六个月发布一次，所以从2018年开始，Java每半年会出现一个新的版本号。目前快速增长到了Java SE 12,2020年3月份计划发布Java SE 13[6][7].

## 参考文献

