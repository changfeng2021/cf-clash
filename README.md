<h1 align="center" dir="auto">使用说明</h1>

## 简介

`长风Clash`是由 `Java`封装的`Clash.Meta`内核，集成了 `Dashboard ui` 和 `yacd` 管理页面，可能轻松实现科学上网常规操作。程序目前只在 Linux 环境测试，也可运行在虚拟机与Docker 环境，建议使用 Docker 部署。

> 其它操作系统目前不支持透明网关功能

### 定位

该程序定位是做透明网关使用，在路由器设置`网关`与`DNS`后供全家设备上网，因此程序不会直接修改系统代理。如果是单机使用建议使用其它的客户端

> 如果家里有树莓派、NAS、闲置电脑可以直接使用本程序，也可安装在虚拟机、Docker

### 使用方法

在 Linux 独立使用，请使用 root 用户执行，如果是 Docker 请使用 `privileged` 如：`docker run --name cf-clash --net=host --privileged cf-clash:v0.1`

> 因为程序是基于 jdk11写的，请先安装 jdk11 环境后再运行.
> 
> ubuntu：sudo apt -y install openjdk-11-jdk-headless
> 
> CentOS:  sudo yum install java-11-openjdk
> 
> Open jdk: https://jdk.java.net/archive/
