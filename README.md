# 数据存储与管理项目

本项目旨在提供一个简单的数据存储与管理解决方案，适用于需要基本文件存储和访问功能的应用场景。

[![License](https://img.shields.io/badge/license-GPL--3.0-blue.svg)](LICENSE)

## 概述

本项目提供了基本的数据存储功能，支持数据的存储、覆盖存储、读取以及删除操作。它适合用于小型应用或者需要简单数据管理的场合。

## 功能特性

- 存储数据到文件
- 覆盖存储已存在的数据
- 从文件中读取数据
- 删除存储的数据文件

## 安装和使用

### 安装

1.将文件放置在网站目录
2.修改授权码和加密码

### 使用[POST请求]

#### 使用 POST 请求存储数据

`curl -X POST 'http://your-domain.com/database.php'
-H 'Content-Type: application/x-www-form-urlencoded'
--data-urlencode 'action=store'
--data-urlencode 'name=cs'
--data-urlencode 'data=Hello World'
--data-urlencode 'authorization_code=AAA'`

#### 使用 POST 请求覆盖已存在的数据

`curl -X POST 'http://your-domain.com/database.php'
-H 'Content-Type: application/x-www-form-urlencoded'
--data-urlencode 'action=store'
--data-urlencode 'name=cs'
--data-urlencode 'data=Updated Data'
--data-urlencode 'authorization_code=AAA'`

### 使用[GET请求]

#### 使用 GET 请求读取数据

`curl -X GET 'http://your-domain.com/database.php?action=retrieve&name=cs&authorization_code=AAA' `

