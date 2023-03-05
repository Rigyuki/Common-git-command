# Common-git-command
# 克隆分支到本地（初次）
git clone -b yuki 'https://github.com/Rigyuki/Ghost.git'

[-b] branch

[yuki] branch name 

[https://github.com/Rigyuki/Ghost.git] remote repository url


# git下拉历史版本
git log                    [找到commit id]
git checkout 3d1adadacq23e2w1e2w21e2s2s    [后面的是commit id号]


# git创建新分支并上传代码
git checkout -b [branch name]         [创建分支的同时切换到该分支上]
git push origin [branch name]         [将新分支推送到github]
例如
$ git checkout -b gh-dev
Switched to branch 'gh-dev'

# git删除分支
git push origin :[branch name]           [分支名前的冒号代表删除]


# LF will be replaced by CRLF the next time Git touches it
git config --global core.autocrlf false



# git分支代码合并到主分支
分支yukiNew

主分支main

此刻处于yukiNew分支中

git checkout main

git pull origin main

git merge yukiNew

git push origin main




# git合并分支时出现“Please enter a commit message to explain why this merge is necessary”报错的解决方法
按键盘上的“i”键可进入插入模式

这时可以修改最上方的黄色部分，改成你想写的合并原因

按键盘上的“Esc”键退出插入模式

最后在最下面输入“ :wq ”后按回车键即可

