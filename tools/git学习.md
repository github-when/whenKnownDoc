[TOC]

# 简单部分

```shell
git add fileName // 添加文件内容改动到暂存区
git add . //所有文件内容更改存到暂存区
git commit -m "commit message" //暂存本地仓库
git push // 推送到远程仓库
git clone // 拉取远程仓库代码
git pull //拉取远程仓库修改到本地
```

# 分支部分

```shell
git branch branchName //创建分支
git checkout branchName //切换分支
git checkout -b branchName //创建分支,并且切换到创建的分支
git branch -d branchName //删除分支
git branch -D branchName //强制删除分支[慎用]
git merge branchName //合并分支到主分支
git push origin branchName //提交内容到分支
```

# 冲突

```shell
git merge --abort //放弃解决冲突
```

# 更改历史和状态

```sehll
git status // 当前修改状态
git log // 代码本地commit记录
git log -p //查看修改的详细状态
git log --stat //查看修改的部分状态
git show SHA-1码// 查看任意一个commit
git show 5e68b0d8 shopping\ list.txt //查看任意一个的其中一个文件的更改
git diff --staged //显示暂存和上一条提交之间的不同
```

