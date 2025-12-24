# Postman使用指南

## 1. 什么是Postman？
- 测试API接口的工具
- 可以发送HTTP请求（GET、POST等）
- 可以查看服务器响应

## 2. 下载安装
访问：https://www.postman.com/downloads/
下载Windows版本，安装

## 3. 基本使用步骤

### 第一步：打开Postman
安装后打开软件

### 第二步：发送第一个请求
1. 点击左上角"New" → "HTTP Request"
2. 在新窗口中：
   - 选择方法：GET
   - 输入URL：https://httpbin.org/get
   - 点击"Send"

### 第三步：查看响应
在下面会显示：
- 状态码：200
- 响应体：JSON格式的数据

## 4. 练习任务
用Postman测试这些URL：

1. GET请求测试：
   https://httpbin.org/get
   https://jsonplaceholder.typicode.com/posts

2. POST请求测试：
   https://httpbin.org/post
   方法：POST
   Body → raw → JSON
   输入：{"test": "hello"}

## 5. 为什么需要Postman？
- 开发时测试API是否正常工作
- 调试时查看详细请求响应
- 保存常用的API测试
