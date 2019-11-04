# Vxlan practice & Flannel

## Vxlan

Virtual Extensible LAN(VXLAN)是一个在三层网络上模拟二层网络的网络虚拟化技术。主要为了解决云计算场景下子网不够用的问题。传统 vlan 只能支持 4000 个子网，vxlan 可以支持 1600 万个子网（Vxlan 网络标识符 VNI 字段为 24 位，2^24 个子网）。

主要技术实现是通过

### Vxlan 介绍

vxlan 的包结构

1. 需要哪些东西才可以把包发出去

### Vxlan practice in linux

## Flannel and vxlan

## Reference
