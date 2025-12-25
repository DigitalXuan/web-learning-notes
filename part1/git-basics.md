# Git与GitHub学习笔记

## 1. Git是什么？
- 分布式版本控制系统
- 记录文件的变化历史
- 方便团队协作开发

## 2. 核心命令

### 基础工作流
```bash
# 初始化仓库
git init

# 添加文件到暂存区
git add 文件名
git add .              # 添加所有文件

# 提交更改
git commit -m "提交说明"

# 查看状态和历史
git status
git log --oneline

# 推送到远程仓库
git push origin main

# 添加远程仓库
git remote add origin git@github.com:用户名/仓库名.git

# 查看远程仓库
git remote -v

# 第一次推送
git push -u origin main
