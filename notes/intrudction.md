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
  
  - 一般有Deployment ReplicaSet DaemonSet StatefuleSet Job 等
    
    -    
