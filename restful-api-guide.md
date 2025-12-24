# RESTful API设计指南
## 1.什么是RESTful API?
- 一种设计Web API的规范
- 把数据看作"资源",用HTTP方法操作
- 比如：用户是资源，文章是资源
## 2.核心规则
### 规则1：用名词不用动词
√ /users    获取用户列表
× /getUsers 获取用户列表
### 规则2：用复数名词
√ /users    用户集合
√ /users/1  用户ID=1
### 规则3：用HTTP方法表达操作
| 操作 |    方法    |          示例          | 
|------|------------|------------------------|
|  查  |    GET     |       GET /users       |
|  增  |    POST    |      POST /users       |
|  改  |    PUT     |      PUT /users/1      |
|  删  |   DELETE   |     DELETE /users/1    |
## 3.博客API示例
### 用户管理
GET      /api/users     #获取所有用户
POST     /api/users     #创建用户
GET      /api/users/1   #获取用户1
PUT      /api/users/1   #更新用户1
DELETE   /api/users/1   #删除用户1
###文章管理
GET      /api/articles    #获取所有文章
POST     /api/articles    #创建文章
GET      /api/articles/1  #获取文章1
PUT      /api/articles/1  #更新文章1
DELETE   /api/articles/1  #删除文章1
## 4.响应格式
### 成功响应
json
{  "success": true,
   "data":{
     "id":1,
     "name": "张三"
  }
}
### 错误响应
{
  "success": false,
  "error": "用户不存在"
}
