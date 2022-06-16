---
footer: true
outline: deep
typora-copy-images-to: upload
---

# 简介

## 什么是 Golang？

Golang（Go 语言） 是谷歌开发的开源编程语言，用于大规模构建快速、可靠和高效的软件。它兼具 Python 等动态语言的开发速度和 C/C++ 等编译性语言的性能和安全性。

起源于 2007 年，2009 年正式对外发布。

下面是一个最基本的示例：

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, World")
}
```

## 创始人

Go 语言的创始人都是 IT 界的超级大神，而且创始时都就职于 Google 公司。

### Ken Thompson（肯·汤普逊）

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202206160021161.png)

  - Unix 之父（他和 C 语言之父丹尼斯·里奇一起开发了 Unix 操作系统）

  - C 语言创始人（C 语言之父和他，在他开发的 B 语言基础上开发了 C 语言)

  - 1983 年获图灵奖

  - UTF-8 编码创始人

### Rob Pike（罗勃·派克）

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202206160021585.png)

- Go 语言项目总负责人
- Unix 的团队成员
- UTF-8 编码创始人
- 参与了[贝尔实验室](https://en.wikipedia.org/wiki/Plan_9_from_Bell_Labs)和[Inferno](https://en.wikipedia.org/wiki/Inferno_(operating_system))操作系统的 Plan 9 的创建，以及[Limbo 编程语言](https://en.wikipedia.org/wiki/Limbo_programming_language)。
- 1980年奥运会射箭的银牌得主
- 业余天文学家

### Robert Griesemer（罗伯特·格瑞史莫）

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202206160022890.png)

  Google V8 JavaScript 引擎、Chubby 和 Java HotSpot JVM 的主要贡献者。

## 为什么要创建 Go 语言？

Google 大量使用 C++，Go 语言创始人觉得 C++ 在大规模开发中使用起来太慢、太麻烦了、太复杂了，这些大佬深知 C++的问题：

- 软件复杂：多核处理器、网络系统、大规模计算集群和网络编程模型所带来的问题只能暂时绕开，没法根本解决。
- 软件规模：Google 的服务器程序由千万行代码组成及大量程序员协作开发，软件规模非常之大，同时要求更新速度快，而 C++ 无法满足。
- 编译慢：C++虽然运行速度快，但在大型编译集群中，构建时间延长到了几分钟，甚至几小时。严重影响了工作效率。
- 可读性和易用性都不如动态语言 Python 和 JavaScript。C++ 真的太复杂了。

Go 语言的所有设计者都说，设计 Go 语言是因为 C++ 给他们带来了挫败感。在 Google I/O 2012 的 Go 设计小组见面会上，Rob Pike 是这样说的：

> 我们做了大量的 C++ 开发，厌烦了等待编译完成，尽管这是玩笑，但在很大程度上来说也是事实。

但 C++历史包袱太重，很难从根本上去解决，于是他们就想创建一门新的编程语言。

## 历史

### 2007 年开始设计

三位创始人于 2007 年开始设计 Go。


### 2009 年正式推出

Go 于 2009 年 11 月正式宣布推出并开源，并在 Linux 及 Mac OS X 平台上进行了实现，后来追加了 Windows 系统下的实现。

### 2012 年 3 月 Go 1.0

随着 Go 第一个版本发布的还有一份兼容性说明文档。该文档说明，Go 的未来版本会确保向后兼容性，不会破坏现有程序。

此版本中已经包含 go tool pprof 命令，它是[Google的pprof C++分析器](https://github.com/gperftools/gperftools)的一个变种；同时还包含 go vet 命令（之前的是 go tool vet），它可以报告程序包中可能存在的错误。

之后，Go 广泛应用于 Google 的产品以及许多其他组织和开源项目。

### 2013 年 5 月 Go 1.1

从 2013 年开始 Go 每半年发布一个二级版本（即从a.x升级到a.y）。

这个版本的 Go 致力于增强语言特性（编译器、垃圾回收机制、映射、goroutine 调度器）与性能。

此版本内置了[竞态检测器](https://blog.golang.org/race-detector)，这已成为 Go 语言必不可少的工具。*你可以通过这篇文章：“*[*Race Detector with ThreadSanitizer*](https://medium.com/@blanchon.vincent/go-race-detector-with-threadsanitizer-8e497f9e42db)*” 了解更多关于竞态检测器的信息。*

重新编写后的[Go的调度器](https://docs.google.com/document/d/1TTj4T2JO42uD5ID9e89oa0sLKhJYD0Y_kqxDv3I3XMw/edit)性能有了显著提高。

### 2013 年 12 月 Go 1.2

test 命令支持代码覆盖率报告，并提供新的 go tool cover 命令输出代码测试覆盖率的统计信息：

![img](https://static001.infoq.cn/resource/image/82/94/8200ab6e62e1b21e75e31a0551e93194.png)

### 2016 最佳语言

在2016年，Go被软件评价公司TIOBE 选为“TIOBE 2016 年最佳语言”。

### 目前

目前最新稳定版本为 [1.18.3](https://go.dev/doc/devel/release)。

## Go 语言吉祥物

Go 语言有一个吉祥物，在会议、文档页面和博文中，大多会包含下图所示的图标。

![](http://c.biancheng.net/uploads/allimg/180808/1-1PPQA9545W.jpg)

它其实是迪士尼动画中的人物 Gopher。这是才华横溢的插画家 Renee French 设计的，她也是 Go 设计者之一 Rob Pike 的妻子。

![image-20220616013310348](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202206160133382.png)

