
一图胜千言

![iamge](https://github.com/BevanHuang/learn-git/blob/master/Image/AboutGit.png)


配置
-----
git config --global user.name "<姓名>" 设置提交者姓名。<br>
git config --global user.email "<邮箱>" 设置提交者邮箱。<br>

基础操作
-----
git init [目录名] 在指定目录创建仓库，如果没有指定目录名将在当前目录创建仓库。<br>
git clone <远程仓库地址> [目录名] 从指定地址克隆仓库，若不指定目录名将默认创建与远程同名目录。<br>
git add <目录名|文件名> 将文件或目录中已修改的代码添加追暂存区。<br>
git commit -m "<注释>" 提交暂存区内容。<br>
git status 查看仓库状态<br>

比对 diff
-----
git diff 比对当前内容和暂存区内容。<br>
git diff HEAD 比对当前内容和最近一次提交。<br>
git diff HEAD^ 比对当前内容和倒数第二次提交。<br>
git diff HEAD^ HEAD 比对最近两次提交。<br>

历史 log
-----
git log [--oneline] [--all] 查看提交历史。<br>
git log --oneline 打印为单行log。<br>
git log --all 打印所有记录（忽略HEAD的位置）。<br>
git log --graph 打印示意图（忽略HEAD的位置）。<br>

分支 branch
-----
git branch [分支] 有分支：创建分支，无分支：列出所有分支。<br>
git checkout <分支> 切换至分支。<br>
git checkout -b <分支> 创建并切换至分支分支。<br>
git merge <分支> 将分支与当前分支合并。<br>

远程
-----
git pull 拉取远程仓库。<br>
git push <远程仓库> <分支> 推送至远程仓库。<br>
git remote add origin https://xxx.git 新增远程仓库origin<br>
git remote set-url origin https://xxx.git 修改远程仓库origin<br>
