Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes.
Git tracks changes of files.

学习步骤：
git init 初始化库
git add .                       ---》这一步就是将文件从工作区移到暂存区
git commit -m"文件描述"          ---》这一步就是提交更改，实际上就是把暂存区的所有内容提交到当前分支
git log         -->查看更改版本
git reset  --hard commit-id（需要退回到哪个版本就用哪个）
命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
    一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
    一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
    (git checkout -- file命令中的--很重要，没有--，就变成了“切换到另一个分支”的命令，我们在后面的分支管理中会再次遇到git checkout命令。)