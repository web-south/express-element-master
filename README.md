# HTML CSS 实战项目分析说明

+ 项目源码：https://github.com/web-south/express-element-master

## 1. 项目环境搭建

### 1.1 项目初始化

+ 项目初始化

  ```bash
  npm init -y
  ```

### 1.2 下载安装第三方模块

+ 本地下载安装项目所需第三方模块

  ```bash
  npm install express --save
  ```

### 1.3 创建项目服务器

+ 创建服务器： app.js

  ```js
  //1. import express
  const express = require('express')

  const path = require('path')

  //2. create express server
  const app = express()

  //5.open express static resource: public
  app.use(express.static(path.join(__dirname, 'public')))

  //6.express static resource: views
  app.set('views', path.join(__dirname, '/views'))

  //3.config port and listen port:3000
  const PORT = process.env.NODE_ENV || 3000
  app.listen(
    PORT,
    console.log(`Server linten on port:http://localhost:${PORT}...`)
  )
  ```

+ 测试: 浏览器 url 分别输入

  ```bash
  localhost:3000              
  ```

### 2.1  Page of Home

#### 2.1.1 header section

+ 详见 02-layout_header.html

#### 2.1.2 layout 

+ 详见 01-layout.html

#### 2.1.3  footer section

+ 详见 04-layout_footer.html

#### 2.1.4 main section

+ 详见 03-layout_main.html


### 


