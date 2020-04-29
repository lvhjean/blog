---
title: NPM查看包的版本信息
date: 2020-04-16 14:06:28
tags: npm
---

> 分两种情况,NPM命令可以查看npmjs服务器上的包的版本信息,也可以查看本地安装的包的版本信息.

## 查看npmjs服务器上的包的版本信息

1. npm view pkg version 查看服务器上包pkg的最新的版本信息
    ```
    npm view gulp version 
    4.0.0
    ```
2. npm view pgk versions 查看npmjs服务器上包pkg的所有的版本信息
    ```
    npm view gulp versions
    ```
3. npm info pkg 查看npmjs服务器上包pkg的最新的版本信息,和npm view pkg version的功能类似,但比npm view pkg version提供的信息更丰富
    ```
    npm info gulp
    ```

## 查看本地安装包的版本信息

1. npm ls pkg 查看某个项目下包pkg的版本信息,注意该命令需要在某个项目下执行
    ```
    npm ls webpack
    webapp_backend@1.0.0 /本地的项目路径
    └── webpack@3.12.0 
    ```
2. npm ls pkg -g 查看本地全局安装的pkg版本
    ```
    npm ls webpack -g
    /Users/mac/.nvm/versions/node/v8.8.0/lib
    └── webpack@4.29.6
    ```
