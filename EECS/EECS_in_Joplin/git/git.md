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
git commit -m “对当前版本的描述”
 
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



### 3. 多台设备的基本流程

- 在A电脑

  ```shell
  1.克隆远程仓库代码
  	git clone 远程仓库地址（内部已实现 git remote add origin 远程仓库地址）
  	
  2.切换分支
  	git checkout 分支
  ```

  

- 在B电脑中

  ```shell
  1.切换到分支进行开发（比如dev分支）
  	git checkout dev
  	
  2.拉取代码
  	git pull origin dev
  	
  3.继续开发
  4.提交代码
  	git add .
  	git commit -m ''
  	git push origin dev
  ```

  

- 继续在A电脑中

  ```shell
  1.切换到分支进行开发（比如dev分支）
  	git checkout dev
  	
  2.拉取代码
  	git pull origin dev
  	
  3.继续开发
  4.提交代码
  	git add .
  	git commit -m ''
  	git push origin dev
  ```

- 开发完毕，合并dev 分支到 master 分支

  ```shell
  1.将 dev 分支合并到 master 进行合并
  	git checkout master
  	git merge dev
  	git push origin master
  	
  2.把dev 分支也推送到远程
  	git checkout dev
  	git merge master
  	git push origin dev
  ```

  

