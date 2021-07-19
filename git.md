# Git

```
git config --global user.name '名字'
git config --global user.email 邮箱

git init //本地初始化
git add xx//添加文件到暂存区
git status //查看暂存区状态
git commit -m '备注' //提交
git log //查看日志
git diff HEAD -- xx //将暂存区文件与版本库内容对比
git reset HEAD //撤销提交到暂存区的文件
git log -几个 --pretty=oneline //日志输出几个，在一行显示
git reset --hard HEAD^ //回退一个版本
git reset --hard HEAD~10 //回退十个版本
git reset --hard 版本号 //到指定版本
cat 文件名 //查看文件内容
git reflog //查看log历史记录
git checkout -- 文件名 //本地文件误删除，从本地版本库恢复
git rm 文件名 //删除本地和本地版本库
git ls-files //查看本地版本库文件

git remote add origin https://github.com/xxx //绑定远程仓库
git push -u origin main //推送

git branch //查看所有分支
git checkout -b xxx //创建并切换到分支 --会clone主分支的所有内容
git checkout xxx //切换到指定分支
git merge xxx //合并分支 --只能在主分支上合并
git branch -d xxx //删除分支
git branch -m 原来分支名字 更改的名字 //更改分支名字 --M是强制重命名

先添加到暂存区--再提交到版本库--推送到远程
git branch -a //查看本地和远程仓库
git push origin xxx //推送分支到远程仓库
git push origin :xxx //删除远程仓库分支（本地仓库会保留）
git fetch origin //同步远程分支到本地
git checkout -b leaf02 origin/leaf02 //拉取远程分支到本地

git pull //拉取远程仓库 -- 解决多人开发上传问题
git push //提交到远程仓库

git tag //查看tag
git tag xxx //设置标签（发行版本）
git tag -a v_0.1.1 -m 'bug修复' //添加tag到暂存区
git push origin v_0.1.0 //推送tag仓库
git push origin V_0.1.1 //删除远程tag
git tag -d xxx //删除本地标签
```

