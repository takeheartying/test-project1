这是我的git命令行测试哦--梁晓莹
基础git:
  git init                               新建本地仓库
  git add .                              添加到暂存区
  git commit -m "content"                把暂存区的所有内容提交到当前分支[默认第一个分支：master]

  git log --pretty=oneline
  git log --oneline
  git log

  git reset --hard xxxx[commit_id]
  git reset --hard HEAD^
  git reset --hard HEAD^^
  git reset --hard HEAD~100
  git reflog

