# flexDemo
flex布局学习笔记和实例
git push <远程主机名> --delete <远程分支名>
git push <远程主机名> <本地分支名> ：<远程分支名>
git pull 命令
作用：取回远程主机某个分支的更新，再与本地的指定分支合并

格式：git pull  <远程主机名> <远程分支名>:<本地分支名>

1. 如果与当前分支合并，则可省略本地分支名

git pull <远程主机名> <远程分支名> 

相当于：git fetch <远程主机名> <远程分支名>

        git merge <远程主机名>/<远程分支名>

2. 如果当前分支与远程分支存在追踪关系

git pull <远程主机名>

3. 如果当前分支只有一个追踪关系

git pull

4. 手动建立追踪关系

git branch --set-upstream master origin/next

5. 清理远程已删除本地还存在的分支

git fetch --prune origin

或者 git fetch -p

或者 git pull -p