---
title:  安装cnpm
tags:
- npm
---
## npm和cnpm

`npm`包括`npm工具`和`npm仓库`。

`cnpm`包括`cnpm工具`和`cnpm仓库`。

他们的`含义如下`：

- `npm仓库` -  依赖库，服务器在国外。
- `cnpm仓库` - `npm仓库`的镜像，服务器在国内。
- `npm工具` - 用于下载`包`，默认去`npm仓库下载`。你可以`配置registry(临时、永久)`，从而从`registry中下载`。
- `cnpm工具` - 去`cnpm仓库`下载`依赖`



## 安装

首先，配置`npm`的`包安装目录(安装在本地什么位置)`、`缓存目录`。

```shell
# 给npm配置包、缓存目录
# npm config set prefix/cache
# 包存储目录
npm config set prefix 'H:\data\nodejs\node_global'
# 
npm config set cache 'H:\data\nodejs\node_cache'

# 把包目录，添加到NODE_PATH环境变量
NODE_PATH =  H:\data\nodejs\node_global
```
安装`cnpm`。

- `--registry` - 表示让`npm工具`去`cnpm仓库`下载`cnpm工具`

```shell
# 去regisyry仓库下载、安装cnpm
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

