# docker入门与实战（二）

## Docker介绍

#### Docker是一个开源的引擎，可以轻松的为任何应用创建一个轻量的、可移植的、自给自足的容器。开发者在开发环境上编译测试通过的容器可以批量的在生产环境中部署，包括VMS(虚拟机)、bare metal、OpenStack集群和其他基础应用平台。



#### Docker通常用于如下环境

- web应用的自动化打包和发布
- 自动化测试和持续集成、发布
- 在服务环境中部署和调整数据库或其他后台应用
- 从头编译或者扩展现有的OpenStack或Cloud Foundry平台来搭建自己的pass环境



#### Docker VS VM

##### VM

- 运行在宿主机上的完整操作系统
- 运行自身系统会占用较多的资源



##### Docker

- Docker更加轻量高效
- 对系统资源利用率很高
- 比虚拟机技术更为轻便、快捷
- 隔离效果不如VM



#### Docker相关概念

##### Docker是CS架构，主要有两个概念

Docker daemon:

- 运行在宿主机上
- Docker守护进程
- 用户通过Docker client(Docker命令) 与 Docker daemon交互



Docker client

- Docker命令行工具，是用户使用Docker的主要方式
- Docker client 与 Docker daemon通信并将结果返回给用户
- Docker client 也可以通过socket 或 RESTful api 访问远程的 Docker daemon



#### Docker运行过程

先有镜像(image)，后有容器(container) <br>

镜像（相当于exe程序，静态的, 分层的）转化为  容器（进程，动态的）

运行 ( run ) 容器



#### DockerFile
相当于 npm 的 package.json文件，用于存放配置文件的

