Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.



学习步骤：
git init 初始化库
git add .                       ---》这一步就是将文件从工作区移到暂存区
git commit -m"文件描述"          ---》这一步就是提交更改，实际上就是把暂存区的所有内容提交到当前分支
git log         -->查看更改版本
git reset  --hard commit-id（需要退回到哪个版本就用哪个）