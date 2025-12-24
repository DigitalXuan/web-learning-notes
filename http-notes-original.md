# HTTP协议核心概念

## 1. HTTP是什么？
- 超文本传输协议(HyperText Transfer Protocol)
- Wed通信的基础，客户端-服务器模型
- 基于请求(Request)和响应(Response)

## 2. HTTP请求方法(最常用5个)

### GET - 获取资源
```
GET /api/users HTTP/1.1
Host: api.example.com
```
用途：获取数据，参数在URL中，不应修改服务器状态
### POST - 创建资源
POST /api/users HTTP/1.1
Content-Type: application/json
{name: 张三，age: 25}
用途：提交数据，创建新资源
