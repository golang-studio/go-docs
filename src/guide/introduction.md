---
footer: true
outline: deep
typora-copy-images-to: upload
---

# 简介

## 什么是 Golang？

Golang 是谷歌开发的开源编程语言，用于大规模构建快速、可靠和高效的软件。

起源于 2007 年，2009 年正式对外发布。

它兼具 Python 等动态语言的开发速度和 C/C++ 等编译性语言的性能和安全性。

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

## 历史

### 2007 年开始设计

上面三位创始人与 2007 年开始设计 Go。

其目的在于提高在[多核](https://zh.wikipedia.org/wiki/多核心處理器)、网络机器（networked machines）、大型[代码库](https://zh.wikipedia.org/wiki/代码库)（codebases）的情况下的开发效率，以满足 Google 需求。为了解决其他语言使用中的缺点，但是仍保留他们的优点。因此，他们希望设计这样一门语言：

- 静态类型和[运行时](https://zh.wikipedia.org/wiki/运行时)效率。（如：[C++](https://zh.wikipedia.org/wiki/C%2B%2B)）
- 可读性和易用性。（如：[Python](https://zh.wikipedia.org/wiki/Python) 和 [JavaScript](https://zh.wikipedia.org/wiki/JavaScript)）
- 高性能的网络和[多进程](https://zh.wikipedia.org/wiki/多进程)。

设计师们主要受他们之间流传的“不要像C++”启发。  
Go 语言的所有设计者都说，设计 Go 语言是因为 C++ 给他们带来了挫败感。在 Google I/O 2012 的 Go 设计小组见面会上，Rob Pike 是这样说的：

> 我们做了大量的 C++ 开发，厌烦了等待编译完成，尽管这是玩笑，但在很大程度上来说也是事实。


### 2009 年正式推出

Go 于 2009 年 11 月正式宣布推出并开源，并在 Linux 及 Mac OS X 平台上进行了实现，后来追加了 Windows 系统下的实现。

### 2012 年发布 1.0 版本

版本 1.0 在 2012 年 3 月发布。之后，Go 广泛应用于 Google 的产品以及许多其他组织和开源项目。

### 2016 最佳语言

在2016年，Go被软件评价公司TIOBE 选为“TIOBE 2016 年最佳语言”。

### 目前

Go 每半年发布一个二级版本（即从a.x升级到a.y）。

目前最新稳定版本为 [1.18.3](https://go.dev/doc/devel/release)。

## Go 语言吉祥物

Go 语言有一个吉祥物，在会议、文档页面和博文中，大多会包含下图所示的图标。

![](http://c.biancheng.net/uploads/allimg/180808/1-1PPQA9545W.jpg)

它其实是迪士尼动画中的人物 Gopher。这是才华横溢的插画家 Renee French 设计的，她也是 Go 设计者之一 Rob Pike 的妻子。

![image-20220616013310348](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202206160133382.png)

