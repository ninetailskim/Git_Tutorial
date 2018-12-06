Git is a vresion control system.
Git is free software.
Git is a distributed version control system.
Git is free software distributed under the GPL.

git remote add origin XXXXXX

git push -u origin master

git checkout -b dev


git checkout 
-b 表示创建并切换，相当于
    git branch dev
    git checkout dev


git branch 查看当前分支, 列出所有分支，当前分支有星号
-d 删除指定分支


git merge A 合并A分支到当前分支

Creating a new branch is quick & simple.

Creating a new branch is quick AND simple.

???feature1???

所以在merge的时候要先切回要merge入的分支！

用 --no-ff 合并时可以保留原分支，之前的不会保留分支

git stash 保存现场

git remote 

因此，多人协作的工作模式通常是这样：

首先，可以试图用git push origin <branch-name>推送自己的修改；

如果推送失败，则因为远程分支比你的本地更新，需要先用git pull试图合并；

如果合并有冲突，则解决冲突，并在本地提交；

没有冲突或者解决掉冲突后，再用git push origin <branch-name>推送就能成功！

如果git pull提示no tracking information，则说明本地分支和远程分支的链接关系没有创建，用命令git branch --set-upstream-to <branch-name> origin/<branch-name>。