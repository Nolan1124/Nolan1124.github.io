# Git常用命令整理

1. git push <远程主机名> <本地分支名>：<远程分支名>：提交到远程分支

2. git checkout -b <new_branch>: 创建并切换到新分支 （git push只推送当前分支到远程关联分支）

3. git config:git配置命令
config 配置有system级别、global（用户级别）、和local（当前仓库）三个，设置先从system-》global-》local  底层配置会覆盖顶层配置 分别使用--system/global/local 可以定位到配置文件

（1）查看系统config
git config --system --list
　　
（2）查看当前用户（global）配置
git config --global --list

（3）查看当前仓库配置信息
git config --local --list

（4）配置用户名
git config --global user.name "myname"

（5）配置邮箱
git config --global user.email "test@gmail.com"

4. git remote add origin <远程仓库名>：关联远程仓库
