# 微博/推特类API设计

## 用户模块
POST /api/register    # 注册
POST /api/login       # 登录
GET  /api/profile     # 个人资料

## 动态模块  
POST /api/tweets      # 发布动态
GET  /api/tweets      # 获取动态流
POST /api/tweets/{id}/like  # 点赞
