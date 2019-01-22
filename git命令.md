# 迁移SVN #
git svn clone

git remote add origin 

git pull --rebase origin master

<<<<<<< HEAD
git push -u origin --all


# git常用命令 #

## 版本回退 ##

- git reset --hard commit_id 回退版本
- git log 查看提交历史，
- git reflog 查看命令历史
- git checkout -- file 丢弃工作区修改
- git reset HEAD <file> 丢弃暂存区修改
- git rm 用于删除一个文件

## 远程仓库 ##
- git remote add origin git@server-name:path/repo-name.git 关联一个远程库
- git push -u origin master 第一次推送master分支的所有内容，并把本地master关联到远程
- git push origin master 推送最新修改；
- git clone 克隆远程仓库

## 分支管理 ##
- 查看分支：git branch
- 创建分支：git branch <name>
- 切换分支：git checkout <name>
- 创建+切换分支：git checkout -b <name>
- 合并某分支到当前分支：git merge <name>
- 删除分支：git branch -d <name>
=======
>>>>>>> d70c435bf17501e5345070e9a8c8b57531715a13

