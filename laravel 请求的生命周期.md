---
title: laravel 请求的生命周期
tags:
  - php
  - laravel
categories: 学习
top: false
date: 2024-12-09 14:56:35
---
# laravel 请求的生命周期
## 1、接收请求

在 laravel 中所有请求的入口点都是 `public/index.php` 文件。这些请求都需要你的 web 服务器（Apache/Nginx）配置定向到此入口。 `index.php` 是加载框架其余部分的起点。`index.php` 文件将加载 Composer 生成的自动加载器定义，然后从 `bootstrap/app.php` 中检索 Laravel 应用程序的实例。Laravel 本身采取的第一个操作是创建应用 / 服务容器 的实例。
