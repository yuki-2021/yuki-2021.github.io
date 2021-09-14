---
title: npm设置
tags:
- npm
---
## 设置缓存/包路径

用`npm config set prefix/cache`来设置。

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

## 设置registry

两种设置方式。

- `npm install --registry` -  临时去`registry下载安装`
- `npm config set registry xxx` - 永久设置`registry`。可以用`nrm代替`
- `npm config get registry` - 查看`registry地址`

临时使用

```shell
npm install cnpm -g --registry https://registry.npm.taobao.org/
```

永久设置`registry`

```shell
# 永久设置registry 
npm config set registry https://registry.npm.taobao.org/
# 获取registry地址
npm config get registry 
```

