# 产品概述

蓝鲸容器服务(BCS，Blueking Container Service)是高度可扩展、灵活易用的容器管理服务。蓝鲸容器服务支持两种不同的集群模式，分别为原生 Kubernetes 模式和基于 Mesos 自研的模式。使用该服务，用户无需关注基础设施的安装、运维和管理，只需要调用简单的 API，或者在页面上进行简单的配置，便可对容器进行启动、停止等操作，查看集群、容器及服务的状态，以及使用各种组件服务。用户可以依据自身的需要选择集群模式和容器编排的方式，以满足业务的特定要求。

了解蓝鲸容器服务，会涉及到一下基本概念：
* 集群：是指容器运行所需要的物理机或虚拟机资源的集合，可以选择集群的模式是 Kubernetes 或者 Mesos
* 节点：一台已经注册到集群中的服务器
* 应用：由一组容器及服务构成集合，这个集合可以代表一个业务，或者业务的某个大区
* 配置：在配置里面可以定义命名空间和配置模板，它们可以帮助用户管理如何启动容器
* 网络：主要包含**服务**和**负载均衡器**的定义和管理，服务是由多个相同配置的容器和访问这些容器的规则组成的微服务，负载均衡器定义了访问规则的具体实现
* 资源：资源中可以定义业务配置项，通过配置模板中关联这些业务配置项，可以实现对容器中业务进程使用配置的个性化管理
* 仓库：用户存放 Docker 镜像，Docker 镜像用户部署容器服务

## 容器服务怎么用

见下图，只需要三步即可运行服务：
1. 创建集群
2. 创建配置模板集
3. 实例化配置模板集

![](resource/bcsusage.jpg)
