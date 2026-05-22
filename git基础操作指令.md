# Git 常用指令精简速查

## 一、仓库基础

1. `git init` 初始化本地仓库
2. `git clone 仓库地址` 克隆远程仓库到本地
3. `git remote -v` 查看关联的远程仓库
4. `git remote add origin 地址` 绑定远程仓库

## 二、文件提交

1. `git status` 查看文件变动状态
2. `git add 文件名` 单个文件加入暂存
3. `git add .` 所有变动文件加入暂存
4. `git commit -m "备注"` 提交版本并写说明
5. `git log` 查看提交历史记录

## 三、推拉代码

1. `git push` 本地代码上传远程
2. `git push -u origin 分支名` 首次推送绑定分支
3. `git pull` 拉取远程最新代码到本地

## 四、分支操作

1. `git branch` 查看所有本地分支
2. `git branch 分支名` 新建分支
3. `git checkout 分支名` 切换分支
4. `git checkout -b 分支名` 新建并立刻切换分支
5. `git merge 分支名` 合并指定分支到当前分支
6. `git branch -d 分支名` 删除本地分支

## 五、文件删除

1. 手动删本地文件 → `git add .` → 提交推送，远程同步删除
2. `git rm 文件名` 本地 + 仓库一同删除
3. `git rm --cached 文件名` 仅仓库移除，保留本地文件

## 六、配置相关

1. `git config --global user.name 用户名` 设置全局用户名
2. `git config --global user.email 邮箱` 设置全局邮箱
3. `git config --global --list` 查看所有全局配置