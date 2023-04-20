# GIT的快速入门

## 1. 本地操作

```shell
/* git 的初始化，让 git 进入本地文件夹进行管理 */
git init

/* 查看工作区文件的状态 */
git status

/* 切换分支，或者切换文件工作区 */
git checkout

/* 回退所有内容到上一个版本 */
git reset HEAD

/* 添加工作区的文件到暂存区 */
git add [文件名]
git add .
git add *
以上添加以实际情况来操作

/* 个人配置 */
git config --global user.email "xxx"
git config --global user.name "xx"

/* 提交版本 */
git commit - m '对当前版本的描述'

/* 查看版本信息 */
git log
git relog	// 可查看回滚操作的回滚前的版本

/* 回滚 */
git reset --hard commit 版本号

/* 分支操作 */
git branch
git branch 分支名
git checkout 分支名

/* 合并分支 */
git merge 分支名

/* 删除分支 */
git branch -d 分支名


```

## 2. 远程仓库

```shell
/* 给远程仓库起名 */
git remote add 名字 远程仓库地址

/* 向远程仓库推送代码 */
git push -u 名字（默认是origin）分支名

/* 拉取代码 */
git clone 远程仓库地址
git pull 名字 分支

```

