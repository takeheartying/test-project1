这是我的git命令行测试哦--梁晓莹
基础git:
  git init                               新建本地仓库
  git add .                              添加到暂存区
  git commit -m "content"                把暂存区的所有内容提交到当前分支[默认第一个分支：master]
  git rm -- xxxx[Path+file]

  先有本地库，后有远程库的时候，如何关联远程库:
  git remote add origin git@github.com:takeheartying/test-project1.git     本地仓库关联远程仓库【远程库默认名字origin】+ 创建主分支
  git pull origin master --allow-unrelated-histories                       把本地仓库的变化连接到远程仓库主分支
  git push -u origin master                                                把本地仓库的文件推送到远程仓库

  先创建远程库后从远程库克隆:
  git clone xxxx


  git push origin <tagname>              可以推送一个本地标签
  git push origin --tags                 推送所有本地标签
  git tag  -d <tagname>                  删除本地标签
  git push origin :refs/tags/<tagname>   删除远程标签

  git branch                             获取分支
  git tag <name> [commit_id]             打标签----   -a指定标签名，-m指定说明文字
  git tag                                查看标签
  git show <tagname>                     查看标签信息
  git tag -d <tagname>                   删除本地标签


  git checkout -- xxxx[Path+file]        让这个文件回到最近一次git commit或git add时的状态

  git branch <branch_name>               新建branch_name分支
  git checkout <branch_name>             转到branch_name分支
  相当于：
  git checkout -b <branch_name>


  git diff                               工作区和暂存区比较---修改之后还没有暂存起来的变化内容
  git diff --cached                      暂存区和仓库（版本库）的比较---查看已暂存的将要添加到下次提交里的内容
  git diff HEAD -- xxxx[Path+file]       工作区和版本库比较

  git log --pretty=oneline --abbrev-commit
  git log --pretty=oneline
  git log --oneline
  git log -1                             提示最后一次commit信息
  git log

  git reset --hard xxxx[commit_id]       本地仓库（版本库）回滚
  git reset --hard HEAD^
  git reset --hard HEAD^^
  git reset --hard HEAD~100
  git reset HEAD xxxx[file_name]         暂存区（stage）当前内容回滚
  git reflog

