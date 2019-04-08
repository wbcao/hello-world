# hello-world
just another repository

I creat a branch for this repository.


首先，选择一个合适的地方，创建一个空目录：
第二步，通过git init命令把这个目录变成Git可以管理的仓库：

第一步，用命令git add告诉Git，把文件添加到仓库：
$ git add readme.txt

第二步，用命令git commit告诉Git，把文件提交到仓库：

$ git commit -m "wrote a readme file"

$ git commit -a

回退到上一个版本add distributed，就可以使用git reset命令：
$ git reset --hard HEAD^

回到未来的某个版本：
$ git reset --hard 1094a

Git提供了一个命令git reflog用来记录你的每一次命令：git reflog

用git diff HEAD -- readme.txt命令可以查看工作区和版本库里面最新版本的区别：

git checkout -- file可以丢弃工作区的修改：
$ git checkout -- readme.txt
命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：

一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；

一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
总之，就是让这个文件回到最近一次git commit或git add时的状态

git reset HEAD <file>可以把暂存区的修改撤销掉（unstage），重新放回工作区：

git reset命令既可以回退版本，也可以把暂存区的修改回退到工作区。

