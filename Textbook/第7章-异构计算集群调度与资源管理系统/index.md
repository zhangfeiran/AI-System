<!--Copyright © Microsoft Corporation. All rights reserved.
  适用于[License](https://github.com/microsoft/AI-System/blob/main/LICENSE)版权许可-->

# 异构计算集群调度与资源管理系统 (Heterogeneous Computing Cluster Scheduling and Resource Management System)

   

你不能在薄弱的基础上建造一座伟大的建筑。如果你要拥有一个强大的上层建筑，你必须有一个坚实的基础。“You can’t build a great building on a weak foundation. You must have a solid foundation if you’re going to have a strong superstructure.” – Gordon B. Hinckley 

随着工业界和学术界大规模应用人工智能技术，大规模和批量的深度学习模型训练需求变得越来越迫切，各家机构投入重金购置和搭建异构计算集群。其中以配置 GPU（Graphics Processing Unit）加速器和 InfiniBand 网卡的大规模高性能异构计算集群为代表性硬件架构，集群的资源以多租户的形式被组织内的算法工程师使用。集群管理系统（也称作平台）支撑模型的训练，提供作业，数据与模型的管理，并提供资源隔离。如何高效率与稳定的对资源进行管理，是资源管理系统面对的挑战。资源管理系统也是深度学习系统中的基础性系统，企业级场景下，上层框架和应用一般会运行在资源管理系统提供的资源中。

我们回顾一下第一章 1.5 小节的介绍，异构计算的驱动力有暗硅 (Dark Silicon）与异构硬件（Heterogeneous Hardware）的发展趋势。以上两点都会造成数据中心的硬件变的越来越异构，同时应用层面的用户又在多租共享使用硬件，这就产生了抽象与统一管理（Unified Management）的需求。对计算或存储异构硬件，常常抽象在统一的空间内进行管理和池化，最终达到对用户透明。异构计算集群调度与资源管理系统在人工智能系统中类似传统 ***操作系统(Operating System)*** 作用，它对下抽象异构资源（例如，GPU，CPU等），对上层的深度学习作业进行调度和资源分配，在启动作业后也要提供相应的运行时进行资源隔离和环境隔离和作业进程的生命周期管理。

本章将围绕异构计算集群调度与资源管理系统的运行时，调度，存储，开发与运维等内容展开。以期让读者了解，当深度学习生产的问题规模达到多服务器，多租户，多作业的场景，平台系统设计挑战和常用解决方案。



本章包含以下内容：

- [异构计算集群管理系统简介](7.1-异构计算集群管理系统简介.md)
- [作业，镜像与容器](7.2-训练作业，镜像与容器.md)
- [调度](7.3-调度.md)
- [面向深度学习的集群管理系统](7.4-面向深度学习的集群管理系统.md)
- [存储](7.5-存储.md)
- [开发与运维](7.6-开发与运维.md)



```toc
:maxdepth: 2
:numbered:

7.1-异构计算集群管理系统简介
7.2-训练作业，镜像与容器
7.3-调度
7.4-面向深度学习的集群管理系统
7.5-存储
7.6-开发与运维
```
    