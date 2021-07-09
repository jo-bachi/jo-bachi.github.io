# Swarm

> storage and communication infrastructurefor a self-sovereign digital society (自治数字社会的存储和通信基础设施)


Swarm 是一个点对点的节点网络，它们共同提供分散的存储和通信服务。 由于内置激励系统，该系统在经济上是自我维持的，该系统通过以太坊区块链上的智能合约执行并由 BZZ 令牌提供支持。 在本文中，我们首先介绍 Swarm 的网络层，它实现了固定大小的分布式档案 数据单元。 接下来我们描述由 API 提供的高级功能，该功能使 Swarm 成为去中心化 Web 的可行开发堆栈和部署环境。

## Introduction

> Swarm 的使命是通过为去中心化互联网提供可扩展的基础层基础设施，塑造未来走向自主主权的全球社会和无许可的开放市场。

Swarm’s mission is to shape the future towards a self-sovereign global society and permis-sionless open markets by providing scalable base-layer infrastructure for the decentralisedinternet.  Swarm’s vision is to extend the blockchain with peer-to-peer storage and com-munication  to  realise  the  world  computer  that  can  serve  as  an  operating  system  anddeployment environment for decentralised applications.Swarm provides continuity of service and resilience against network outages or targeteddenial  of  service  attacks.   As  a  platform  for  permissionless  publication,  Swarm  fostersfreedom  of  information.   With  its  exceptional  privacy  features  like  anonymous  brows-ing, deniable storage, untraceable messaging and file representation formats that leak nometadata, Swarm responds to the growing demand for security on the web.Built-in incentives seek to optimise the allocation of bandwidth and storage resources andrender Swarm economically self-sustaining.  Swarm nodes track their relative bandwidthcontribution on each peer connection, and excess debt due to unequal consumption canbe settled in BZZ. Publishers in Swarm must spend BZZ to purchase the right to writedata to Swarm and prepay some rent for long term storage.An example of modular design, Swarm consists of clearly separable layers (see figure 1).Technically, (2) and (3) constitute the core of Swarm and are discussed in the followingtwo sections of this paper

 Swarm 的愿景是通过点对点存储和通信扩展区块链，以实现世界计算机，它可以作为分散应用程序的操作系统和部署环境。 Swarm 提供服务的连续性和抵御网络中断或有针对性的拒绝服务的弹性攻击。作为免许可发布平台，Swarm 促进信息自由。凭借其卓越的隐私功能，如匿名浏览、可拒绝存储、不可追踪的消息传递和泄漏 nometadata 的文件表示格式，Swarm 响应了对网络安全性不断增长的需求。内置激励措施旨在优化带宽和存储资源的分配andrender Swarm 在经济上是自给自足的。 Swarm 节点跟踪它们在每个对等连接上的相对带宽贡献，并且由于不均等消耗导致的超额债务可以在 BZZ 中解决。 Swarm 中的发布者必须花费 BZZ 购买将数据写入 Swarm 的权利并预付一些租金以进行长期存储。模块化设计的一个例子，Swarm 由明显可分离的层组成（见图 1）。从技术上讲，（2）和（3）构成 Swarm 的核心，将在本文的以下两节中讨论