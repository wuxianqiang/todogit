# git 使用指南


1. 首先先把我的分支先克隆下来
2. 然后根据master分支创建你自己的分支
3. 然后在你自己的分支中工作，工作完成把你自己的分支推送到远端

# master分支更新
如果master分支更新了，你自己的分支也要更新，使用下面命名
```
git pull --rebase origin master
```
如果有冲突需要自己解决，然后在提交
```
git add .
git commit -m 处理冲突
```
然后退出rebase环境
```
git rebase --continue
```
然后推送到远端即可
```
git push origin master
```
