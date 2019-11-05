ssh-keygen -t rsa -C "youremail@example.com"
home/.ssh
id_rsa      私匙
id_rsa.pub  公匙

a1.git init <dir>

a2.git add <file1 file2 file3>
a3.git commit -m <message>
a4.git checkout -- <file>    撤销工作区的变更

a5.git status                暂存区变更
a6.git diff <file>           显示变更
a7.git diff HEAD^ <file>     上一个版本对比的变更

a8.git log --pretty=oneline
a8.git log --graph --pretty=oneline --abbrev-commit

a9.git reset --hard HEAD^ HEAD^^ HEAD~100  返回之前的版本
b1.git reset HEAD <file> + a4              把暂存区的返回来，HEAD最新版本

b2.git remote add origin url.git           关联远程仓库到本地
b3.git push -u origin <branch>             -u本地分支和远程分支关联
b4.git push origin <branch>                推送到远程的<branch>分支

b5.git checkout -b <branch>                创建并且切换到dev分支
b6.git branch <branch>                     创建分支
b7.git branch -d <branch>                  删除分支
b7.git checkout <branch>                   切换分支
b8.git branch                              查看分支
b9.git merge <branch>                      将<branch>分支合并到当前分支
c1.git merge --no-ff -m "msg" dev          禁止使用ff模式来合并分支
c2.git stash                               存储现场
c3.git stash list
c4.git stash apply {@}
c5.git stash drop  {@}

c6.feature and bug                         功能分支和bug分支处理方式

d1.git remote -v                           查看远程分支和权力
d2.git checkout -b dev origin/dev          创建关联远程dev分支
d3.git pull                                抓取最新的代码
d4.git branch --set-upstream-to=origin/<branch> dev


cat <file>        查看文件
git reflog        命令记录

