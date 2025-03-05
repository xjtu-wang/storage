---
title: 香橙派配置VNC服务器桌面(ubuntu20.04)
date: 2025-03-05 13:15:01
tags: 
---

## 1. 安装x11VNC

``` bash
apt-get update -y
apt-get install x11vnc -y
```

## 2.设置VNC服务器密码
```bash
x11vnc -storepasswd
```

## 3.启动server
```bash
x11vnc -forever -shared -rfbauth ~/.vnc/passwd
```
