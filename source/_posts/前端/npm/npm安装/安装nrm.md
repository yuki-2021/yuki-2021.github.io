---
title:  安装nrm
tags:
- npm
---

## nrm简介

`nrm`两个功能

- 给`npm工具`设置`registry(从哪里下载)`
- 查看`npm工具`的`可用registry`、`正在使用的registry`

## 用法

安装

```shell
cnpm install nrm -g 
```

用`nrm ls`查看`可用registry`

```shell
nrm ls
```

切换`registry`

```shell
 nrm use taobao
```

