## linux git安装及使用
[链接](https://blog.csdn.net/qq_42690368/article/details/82319238)
## git冲突是什么？
## git命令
git branch 查询当前分支
git branch -a 查询本地和远程的所有分支
git branch -r 查询远程的所有分支
git checkout 分支名 切换分支
git checkout -b 分支名 新建分支并切换
git cherry-pick commit-id 合并另一分支的部分代码
git cherry-pick -n commit-id （只更新工作区和暂存区，不产生新的提交）
git remote -v 查看远程主机名
git fetch 远程主机名 拉取远程主机的全部内容到本地
git fetch origin release/1.8:release/1.8 （在本地建立release/1.8分支）
git add . （将修改的文件从工作区添加到暂存区)

## git cherry-pick解决冲突
第一步：git status 查看需要修改的文件
第二步：手动修改文件
目前到这里就结束了

## 问题汇总
hint: not have locally. This is usually caused by another repository pushing解决：push前先git pull 一下,原因未知，待解决，解决的话可以上b站教一下

