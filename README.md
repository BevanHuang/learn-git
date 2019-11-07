![iamge]（https://github.com/BevanHuang/learn-git/blob/master/Image/AboutGit.png)

# learn-git
学习git的笔记：

一、git的作用:
=====
git是版本控制工具

二、git的安装和配置：
=====
官网: http://git-scm.com
官网下载可能有点慢，建议百度下载。

配置：
git config --global user.name "xh"<br>
git config --global user.email "glassysky@126.com"<br>
git config --list 或者 git config -l 查看配置信息<br>

三、git的一些常用命令
=====
git -v 或者 git --version
git 查看命令

四、常用的命令行命令：
=====
    列出所有子目录：
    Unix： ls -la
    Windows: dir/a

cd 文件名  （进入文件）<br>
cd ... （返回上级文件）<br>

  窗口太小可以用jk滚动界面
  j 前进
  k 后退

git的一些命令：
仓库的创建：git init demo 初始化到一个叫demo的自定义文件夹<br>
仓库的拉取：git clone （github的仓库链接） （重命名）<br>
git status （查看仓库当前的状态）<br>

git add .  （将所有修改添加至暂存区）<br>
git commit -m "描述"  （版本提交）（描述特别重要） <br>
commit的内容是暂存区的内容(add操作)，如果add之后有修改了内容，这次修改的内容不会被commit <br>

git log  （查看历史版本）（按 q 退出查看）<br>
git log --oneline // 一行查看<br>
git log -p  // 修改的内容追加到log后面<br>
git checkout 版本的id （版本的id要大于等于7位）<br>
git checkout -  // 回退到上一个节点<br>

git tag -a 标签名 -m "备注"   // 附注标签<br>
git tag  // 列出所有标签<br>
git show 标签名  // 查看标签信息<br>
git checkout 标签名<br>

git branch 分支名 // 创建分支<br>
git checkout 分支名 //切换到分支上<br>
git checkout -b 分支名  // 创建分支并切换到该分支上<br>
git merge 分支名 // 把分支合并到主分支（master）上<br>

git log --all --graph  // 图示全部历史记录<br>

git remote add 远程名称 远程地址  // 添加远程仓库<br>
git remote 列出所有远程仓库<br>

git push -u 远程名称 分支名  // 上传代码，代码就保存在github的仓库里面  （本地-->github）<br>
当本地的项目丢失了之后，用 |git -clone 仓库地址 xh（项目名称）| 命令克隆一个仓库       （github-->本地）<br>
git pull  // 获取远程更新<br>
git pull == git fetch && git merge<br>
