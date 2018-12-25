# 迁移SVN #
git svn clone https://172.16.10.231/svn/msonion/trunk/msonion-store

git remote add origin git@172.16.10.230:tiny-feng/msonion-web.git

git pull --rebase origin master

git push origin --all
