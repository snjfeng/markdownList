# 迁移SVN #
git svn clone

git remote add origin 

git pull --rebase origin master

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
- git remote add origin git@server-name:path/repo-name.git 关联一个空远程库
- git push -u origin master 第一次推送master分支的所有内容，并把本地master关联到远程
- git push origin master 推送最新修改；
- git clone 克隆远程仓库
- git remote -v 查询当前远程的版本
- git fetch origin master  获取最新代码到本地
- git log -p master..origin/master 查看版本差异
- git merge origin/master 合并最新代码到本地分支

## 分支管理 ##
- 查看分支：git branch
- 创建分支：git branch <name>
- 切换分支：git checkout <name>
- 创建+切换分支：git checkout -b <name>
- 合并某分支到当前分支：git merge <name>
- 删除分支：git branch -d <name>
- 分支历史 git log --graph --pretty=oneline --abbrev-commit

## 多人协作 ##
- 远程库信息 git remote -v；
- 从本地推送分支 git push origin branch-name
- 本地创建和远程分支对应的分支使用 git checkout -b branch-name origin/branch-name
- 建立本地分支和远程分支的关联 git branch --set-upstream branch-name origin/branch-name 

## 整理分支 ##
- 变基 git rebase

## 标签管理 ##
- git tag <tagname> 用于新建一个标签，默认为HEAD，也可以指定一个commit id；
- git tag -a <tagname> -m "blablabla..."可以指定标签信息；
- git tag可以查看所有标签。
- git push origin <tagname>可以推送一个本地标签；
- git push origin --tags可以推送全部未推送过的本地标签；
- git tag -d <tagname>可以删除一个本地标签；
- git push origin :refs/tags/<tagname>可以删除一个远程标签。