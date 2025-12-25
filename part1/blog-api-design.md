# 博客系统API设计
## 用户管理
POST  /api/register    #注册
POST  /api/login       #登录
GET   /api/users/{id}  #查看用户
## 文章管理
GET     /api/articles   #文章列表
POST    /api/articles   #发布文章
GET     /api/articles/{id}   #文章详情
PUT     /api/articles/{id}   #修改文章
DELETE  /api/articles/{id}   #删除文章
## 示例
POST /api/articles
Content-Type: application/json
{
  "title": "学习Web开发"，
  "content": "今天学习了HTTP和RESTful API"
}
# 添加并提交
git add blog-api-design.md
git commin -m "添加博客系统API设计"
