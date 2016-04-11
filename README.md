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
