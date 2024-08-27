## SSH

```
ssh-keygen -t rsa -b 4096 -C "happy-yan"
```

### Git

下载代码 git clone xx.git --depth 10 最近十次更新 

[

git submodule update --init --recursive  对于一些很久的分支，要用这个更新一下子模块

git status 查看状态,确定一下是否有没有track的子模块

]

git config --global user.email "xx"

git config --global user.name "xx"

git checkout -b happy/0817_test 复制一个新分支



以下三个都可以用vscode直接运行

git add xx.py

git commit -m "[planner]: add st boundary pre decider test" 添加评论

git push --set-upstream origin happy/0817_test



git reset --soft HEAD^	取消最近的一次更改

git push -f 强制提交



git remote -v 列出现在对于哪一个远程仓库

在同个工作空间中fetch其他仓库：

git remote add origin2 git@github.com:thessshy/Notebook.git

git fetch origin2 --depth 10



`git merge` 用于将两个分支的历史合并。它会创建一个新的合并提交，并保留合并前两个分支的历史。

- 当你在目标分支（如 `main`）上运行 `git merge feature-branch` 时，Git 会将 `feature-branch` 分支的更改合并到当前分支。
- 如果两个分支没有冲突，Git 会自动创建一个新的合并提交，将这两个分支的历史记录结合在一起。
- 如果存在冲突，Git 会要求你手动解决冲突，然后创建合并提交。