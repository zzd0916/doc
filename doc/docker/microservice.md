# docker入门与实战（一）

## 前言-微服务

### 微服务到底是什么

- 微服务属于架构层面的设计模式
- 微服务的设计概念以业务功能为主
- 微服务独立提供对应的业务功能
- 微服务不拘于具体的实现语言
- 微服务架构=模块化开发+分布式计算



### 微服务的特点

- 小，且专注于一件事
- 处于独立的进程中
- 轻量级通信机制
- 松耦合、独立部署



### 合理使用微服务

提前：接口一定是定义清晰的

- 业务复杂度高
- 团队规模大
- 业务需要长期演进
- 最后--没有银弹（没有解决所有问题的灵丹妙药，项目管理，结构设计）



### 微服务--集成与部署

- 持续集成--jenkins
- 虚拟化--虚拟机
- 容器--docker