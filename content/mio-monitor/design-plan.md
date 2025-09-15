---
title: "设计方案"
date: 2025-09-08T00:37:03+08:00
weight: 1
---

mio-monitor 用于 ESP32-C3 端。

## 功能

与 mio-service 建立 websocket 连接。

- 实时获取 PC 设备的硬件状态信息（CPU、内存、IO）。
- 支持对 PC 的一些简单操作（音量、背光亮度）。

## 思路

### 建立连接

1. 终端设备通过 mDNS 广播自身，附加信息用于区分终端设备类型；
2. 终端设备在局域网中扫描广播，发现其他终端设备；
3. 终端 A 向终端 B 发出 pair 请求（pair 由其他路由函数提供），终端 B 同意后，双方建立安全的连接，进行 websocket 通信;
4. mio-monitor 为 ws 服务端，mio-service 为 ws 客户端。

## 技术栈

Rust (esp-idf-hal)
