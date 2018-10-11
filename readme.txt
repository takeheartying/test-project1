这是我的git命令行测试哦--梁晓莹
基础git:
  git init                               新建本地仓库
  git add .                              添加到暂存区
  git commit -m "content"                把暂存区的所有内容提交到当前分支[默认第一个分支：master]
  git rm -- xxxx[Path+file]
  git remote add myorigin git@github.com:takeheartying/test-project1.git 本地仓库关联远程仓库【远程库默认名字origin】


  git checkout -- xxxx[Path+file]        让这个文件回到最近一次git commit或git add时的状态

  git diff                               工作区和暂存区比较---修改之后还没有暂存起来的变化内容
  git diff --cached                      暂存区和仓库（版本库）的比较---查看已暂存的将要添加到下次提交里的内容
  git diff HEAD -- xxxx[Path+file]       工作区和版本库比较

  git log --pretty=oneline
  git log --oneline
  git log

  git reset --hard xxxx[commit_id]       本地仓库（版本库）回滚
  git reset --hard HEAD^
  git reset --hard HEAD^^
  git reset --hard HEAD~100
  git reset HEAD xxxx[file_name]         暂存区（stage）当前内容回滚
  git reflog

