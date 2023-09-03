# git使用
git config --global user.name "用户名"  配置全局用户名
git config --global user.email "邮箱"  配置全局邮箱
git init 初始仓库 在当前目录创建一个.git隐藏文件夹(仓库)
git add test.txt 把文件加进版本控制系统中(暂存区)
git commit 提交(会进入vim编辑器，在里面填写提交声明,会提交到本地仓库)
git commit -m "修改信息" 提交的简化版
git commit -m "fix(test):change context"  git commit的规范(fix表示修改了test文件 后面是修改了什么)

git commit -am"提交信息"中的选项a表示先git add所有发生改动的文件再提交。

git log 查看提交信息
git reset --hard id  回退到某次id提交的那一次 reset表示重置 --hard是重置模式 表示覆盖所有变更
git branch 0.2 创建0.2分支（在此之前要git add 和git commit）
git branch -d 0.2 删除0.2分支

git branch -M main 创建一个main分支并把主分支切换为main

git checkout 0.2 切换到0.2分支
git checkout master 切回主分支
git merge 0.2 合并分支

git remote add origin 仓库地址  绑定远程仓库

git push -u origin master -u 参数相当于是让你本地的仓库和远程仓库进行了关联。第一次push的时候使用

git push <远程主机名> <本地分支名>:<远程分支名> git push origin test:master

如果本地分支名与远程分支名相同，则可以省略冒号： git push <远程主机名> <本地分支名>  git push origin master



