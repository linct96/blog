---
title: common-cmd
date: 2020-08-12 14:51:45
tags: linux
categories:
  - 杂项
---

记录一些不常用又会用到的命令

## GIT

```bash
# 查看git用户信息
$ git config user.name
$ git config user.email

# 设置git用户信息
$ git config --global user.name "zhangsan"
$ git config --global user.email "zhangsan@email.com"

# 设置 git 代理(socks5 和 http 两种方式)
$ git config --global http.proxy 'socks5://127.0.0.1:port' 
$ git config --global http.proxy 'http://127.0.0.1:port'

# 取消 git 代理
$ git config --global --unset http.proxy

```



## NPM

```bash
# 登录npm
$ npm login

# 查看npm用户信息
$ npm whoami

# 查看已安装的package
$ npm list (-g) --depth=0

```


