---
title: "设计方案"
date: 2025-09-14T23:43:40+08:00
weight: 1
---

mio-service 用于 PC 端，并且尽量支持多个操作系统平台。

## 功能

与 mio-monitor 建立 websocket 连接。

- 提供一系列针对 PC 的功能函数。

## 思路

### 控制终端

使用 Rust 的各种 crate 功能对 PC 进行控制：

- **notify-rust**: 桌面通知（跨平台）。

### Agent 进阶

使用 Agent 以及 MCP tools。

将控制各个功能的函数封装成为 MCP tool，使用 Agent 直接解析 JSON 或者自然语言，然后对终端设备进行控制。

## 技术栈

Rust (axum + tokio)
