# learn-git
学习git的笔记：

一、git的作用
git是版本控制工具

二、git的安装和配置：
官网: http://git-scm.com
官网下载可能有点慢，建议百度下载。

配置：
git config --global user.name "xh"
git config --global user.email "glassysky@126.com"
git config --list 或者 git config -l 查看配置信息

三、git的一些常用命令
git -v 或者 git --version
git 查看命令





四、常用的命令行命令：
1.列出所有子目录：
Unix： ls -la
Windows: dir/a

cd 文件名  （进入文件）
cd ... （返回上级文件）

窗口太小可以用jk滚动界面
j 前进
k 后退


git的一些命令：
仓库的创建：git init demo 初始化到一个叫demo的自定义文件夹
仓库的拉取：git clone （github的仓库链接） （重命名）
git status （查看仓库当前的状态）

git add .  （将所有修改添加至暂存区）
git ocmmit -m "描述"  （版本提交）（描述特别重要） 
commit的内容是暂存区的内容(add操作)，如果add之后有修改了内容，这次修改的内容不会被commit 

git log  （查看历史版本）（按 q 退出查看）
git log --oneline // 一行查看
git log -p  // 修改的内容追加到log后面
git checkout 版本的id （版本的id要大于等于7位）
git checkout -  // 回退到上一个节点

git tag -a 标签名 -m "备注"   // 附注标签
git tag  // 列出所有标签
git show 标签名  // 查看标签信息
git checkout 标签名

git branch 分支名 // 创建分支
git checkout 分支名 //切换到分支上
git checkout -b 分支名  // 创建分支并切换到该分支上
git merge 分支名 // 把分支合并到主分支（master）上

git log --all --graph  // 图示全部历史记录
