---
title: "设计方案"
date: 2025-09-08T00:37:03+08:00
weight: 1
---

## 思路

### 建立连接

1. 终端设备通过 mDNS 广播自身，附加信息用于区分终端设备类型；
2. 终端设备在局域网中扫描广播，发现其他终端设备；
3. 终端 A 向终端 B 发出 pair 请求（pair 由其他路由函数提供），终端 B 同意后，双方建立安全的连接，进行 p2p 通信。

### 控制终端

使用 Rust 的各种 crate 功能对 PC 进行控制：

- **notify-rust**: 桌面通知（跨平台）。

### Agent 进阶

使用 Agent 以及 MCP tools。

将控制各个功能的函数封装成为 MCP tool，使用 Agent 直接解析 JSON 或者自然语言，然后对终端设备进行控制。

## 组成

### PC 端

Rust (axum + tokio)

### ESP32 端

esp-idf-hal

### 移动端（测试）

Expo (React Native)

用于替代 ESP32 作为前期测试。
