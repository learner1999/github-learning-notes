# 《GitHub入门与实战》笔记

## 2.5 初始设置

1.设置姓名和邮箱地址
```
git config --global user.name "myname"
git config --global user.email "email@email.com"
```
2.设置color.ui
```
git config --global color.ui auto
```

## 3.1 使用前的准备

1.设置SSH Key
```
ssh-keygen -t rsa -C "email@email.com"
```

## 4.1 基本操作

1.查看提交日志
```
git log --pretty=short #显示提交信息的第一行
git log --pretty=oneline  #每一条commit都显示在一行中
git log -p  #显示文件提交所带来的改动
```

2.查看更改前后的差别
```
git diff  #查看当前工作树和暂存区的区别，如果暂存区没有内容，将会显示工作树和最新提交状态之间的差别
git diff HEAD  #在后面跟上当前指针，比较工作树与最新提交状态之间的差别
```

## 4.2 分支的操作

1.创建并切换分支
```
git checkout -b feature-A  #创建并切换分支
git checkout  #切换分支
git branch    #查看分支，加×号的为当前分支
git checkout -  #用 - 代替分支名，可以切换至上一个分支
```

2.合并分支
```
git merge --no-ff feature-A  #其中的--no-ff表示在历史记录中明确记录下本次分支合并
```

3.图表形式查看分支
```
git log --graph
```
