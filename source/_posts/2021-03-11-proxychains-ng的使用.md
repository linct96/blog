---
title: proxychains-ng的使用
date: 2021-03-11 19:54:58
tags: mac
categories:
  - 杂项
---

## 安装
```bash
brew install proxychains-ng

# 借助代理安装
ALL_PROXY=socks5://127.0.0.1:port brew install proxychains-ng
```

## 修改配置
```bash
# 修改默认配置文件
vim /usr/local/etc/proxychains.conf
```
在最底部添加
```bash
# 通过 socks5 代理
socks5 127.0.0.1 port
```
也可将`socks5`替换为`http`走 http 代理的方式

## 关闭 sip
由于最新的 macos 系统不允许用户修改具有保护权限的文件夹。需要用户进入 recovery 模式 => 实用工具 => 终端 输入如下命令
```sh
# 关闭 sip
csrutil disable
# 开启 sip
csrutil enable
```

