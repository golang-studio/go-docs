---
footer: true
outline: deep
typora-copy-images-to: upload

---

# 著名的 Go 项目有哪些？

Go 语言从发布 1.0 版本以来备受众多开发者关注并得到广泛使用，Go 语言的简单、高效、并发特性吸引了众多传统语言开发者的加入，而且人数越来越多。

使用 Go 语言开发的开源项目非常多。早期的 Go 语言开源项目只是通过 Go 语言与传统项目进行 C 语言库绑定实现，例如 [Qt](http://c.biancheng.net/qt/)、Sqlite 等；后期的很多项目都使用 Go 语言进行重新原生实现，这个过程相对于其他语言要简单一些，这也促成了大量使用 Go 语言原生开发项目的出现。

下面列举的是原生使用 Go 语言进行开发的部分项目。

## Go 语言

[Go](https://github.com/golang/go) 语言自己的早期源码使用 C 语言和汇编语言编写。从 Go 1.5 版本后，完全使用Go语言自身进行编写。Go语言的源码对了解 Go 语言的底层调度有极大的参考意义，建议希望对 Go 语言有深入了解的读者读一读。

## Docker

[Docker](https://github.com/docker/docker) 是一种操作系统层面的虚拟化技术，可以在操作系统和应用程序之间进行隔离，也可以称之为容器。Docker 可以在一台物理服务器上快速运行一个或多个实例。例如，启动一个 CentOS 操作系统，并在其内部命令行执行指令后结束，整个过程就像自己在操作系统一样高效。

## Kubernetes

[Kubernetes](https://github.com/kubernetes/kubernetes) Google 公司开发的构建于 Docker 之上的容器调度服务，用户可以通过 Kubernetes 集群进行云端容器集群管理。系统会自动选取合适的工作节点来执行具体的容器集群调度处理工作。其核心概念是 Container Pod（容器仓）。

## etcd

[etcd](https://github.com/coreos/etcd) 是一款分布式、可靠的 KV 存储系统，可以快速进行云配置。由 CoreOS 开发并维护键值存储系统，它使用Go语言编写，并通过 Raft 一致性算法处理日志复制以保证强一致性。

## beego

[beego](https://github.com/astaxie/beego) 是一个类似 Python 的 Tornado 框架，采用了 RESTFul 的设计思路，使用Go语言编写的一个极轻量级、高可伸缩性和高性能的 Web 应用框架。

## martini

[martini](https://github.com/go-martini/martini) 一款快速构建模块化的 Web 应用的 Go 语言框架。

不过现在已经停止了维护了，难道是 Go 语言的问题？？？😱  
别紧张，请往下看。

## Gin

[Gin](https://gin-gonic.com/zh-cn/) 自称为 Go 语言最快的全功能 Web 框架。晶莹剔透。

它提供类似 Martini 的API，但性能更佳，速度提升高达40倍。如果你是性能和高效的追求者, 你会爱上 Gin。

自然 Martini 不会在维护了啊！😂😂

## 区块链 ethereum

[Go Ethereum](https://github.com/ethereum/go-ethereum) 是以太坊协议的官方 Go 实现。

以太坊是一个运行智能合约的去中心化平台，应用程序完全按照程序运行，没有停机、审查、欺诈或第三方干扰的可能性。

Go Ethereum 是以太坊协议的三个原始实现之一（以及 C++ 和 Python）。它是用 Go 编写的，完全开源并在 GNU LGPL v3 下获得许可。

## 区块链 Hyperledger Fabric

[Hyperledger Fabric](https://github.com/hyperledger/fabric) 是一个企业级许可分布式账本框架，用于开发解决方案和应用程序。其模块化和多功能设计可满足广泛的行业用例。它提供了一种独特的共识方法，可以在保护隐私的同时实现大规模性能。

主要特征：高性能、安全、许可的区块链网络。用 Go 编写的代码，用 Go、Javascript 或 Java 编写的链代码（智能合约），用 Node.js、Java、Go、REST 和 Python 编写的 SDK。

## 等等

还有很多很多……，后续想起来或看到了再更新……