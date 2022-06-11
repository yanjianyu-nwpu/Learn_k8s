# Introduction

## Method

- Cluster 
  
  - 集群

- Master
  
  - 负责调度
  
  - 一个集群可以多个Master，实现高可用

- Node
  
  - 可以就是集群的

- Pod
  
  - Pod 是kubernets 最小的工作单元  每个Pod包含一个或者多个容器
  - Pod提供了比容器更高层次的抽象，更小单位进行抽象调度扩展，
  - Pod 所有容器使用同一个网络namespace 同样的 ip 和port  同样的这样容器可以共享内存，当kubernetes 挂载volume到pod 本质上可将volume 挂载到pod中每个容器‘

- Controller 
  
  - k8s 通常不会直接创建pod 是通过controllker 来管理pod
  
  - 一般有Deployment ReplicaSet DaemonSet StatefuleSes
    
    - Deplyment 是最常用的，可以管理多个副本
    
    - DaemonSet 用于每个Nod最多只
    
    - StatefueSet能保证Pod每个副本 在整个生命周i名称是不变的 而其他controller不提供他   这个功能。
    
    - Job用于运行结束就删除的应用，而其他的controller中的pod通常是长期运行的
    
    - ReplicaSet用于实现pod 多副本管理，

- Service
  
  - Deployment 可以部署多个副本，每个pod 都有自己的ip     
  
  - 通过service 用自己的IP 和 端口， Service 位Pod 提供了负载均衡

- Namespace pod 集群分开    



## Kubernetes Architecture

- Master Node
  
  - Api Server
  
  - Scheduler
    
    - use for decide pod run on which node
    
    - 
  
  - Controller Manager 
  
  - use etcd for memory
