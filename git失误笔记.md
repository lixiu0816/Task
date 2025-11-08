# Git失误笔记

## 远程main分支有本地没有的更新，导致推送被拒绝
1.拉取远程main的更新并合并到本地
`git pull origin main`

2.将本地main分支的内容推送到远程仓库的main分支
`git push origin main`
### 输入完1.的内容后可能会出现下面问题
未跟踪文件与远程仓库拉取下来的文件重名，git就会终止合并操作。
解决步骤：
- 重命名或移到其他目录
`mv "markdown练习.md""markdown.md"`
- 重新执行强制合并
`git pull origin main --allow-unrelated-histories`
注：这时会跳出一个新界面
`1.输入提示信息`
`将鼠标移到只有一个#，后面为空白的地方，输入i，再输入 合并远程main分支与本地main分支。`
`2.保存并退出编辑器`
`先按Esc键，确保处于"命令模式"；`
`再输入 :wq回车`

## 本地分支与远程仓库分支不匹配
### 将master分支的内容推送到main分支中
1.确认本地有没有main分支，执行以下命令
`git branch`
- 如果显示有main分支，直接切换到main分支
`git checkout main`
- 如果没有main分支，则需从当前master分支创建并切换到main分支
`git checkout -b main`

2.将本地提交合并到main分支
`git merge master`

3.推送main分支到远程仓库
`git push -u origin main`
最后再执行一次远程main分支有本地没有的更新，导致推送被拒绝这个步骤的解决方案


