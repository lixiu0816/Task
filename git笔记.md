# Git速查表(Git Cheat Sheet)

## getting started(入门)
1.start a new repo (初始化仓库):

`  git init `

2.clone an exsting repo(克隆已存在仓库):

`git clone <url>`

## prepare to commit(准备提交)
1.add untracked file or unstaged changes(添加未跟踪的文件或未暂缓的文件):

`git add <file>`

2.add all untracked files and unstaged changes(添加所有未跟踪的文件和未暂存的文件):

`git add`

3.choosse which parts of a file to stage(选择文件部分内容暂存):

`git add -p`

4.move file(移动文件):

`git mv <old> <new>`

5.delete file(删除文件):

`git rm <file>`

6.tell git to forget about a file without deleting it(告诉git忽略某个文件):

`git rm --cached <file>`

7.check what you added(查看已缓存的内容):

`git status`

## Make commits（提交更改）
1.make a commit (and open text editor to write message)(提交并打开文本编辑器写提交信息):

`git commit`

2.make a commit(提交直接写信息):

`git commit -m 'mesage'`

3.commit all unstaged changes(提交所有未暂缓的文件):

`git commit -am 'message'`

## Move between branches(分支操作)
1.switch branches(切换分支):

`git checkout <name>`

2.create a branch(创建分支):

`git checkout -b <name>`

## Push your changes(推送更改)
1.push the main branch to the remote origin(将main分支推送至远程origin仓库):

`git push origin main`

2.push a branch that you have never pushed before(推送从未推送过的新分支):

`git push -u origin <name>`

3.push tags(推送标签):

`git push --tags`

4.push the current branch to its remote"tracking branch(将当前分支推送到其远程“跟踪分支”):

`git push`

## Pull changes(拉取更改)
- fetch changes and then merge them into your crrent branch(获取更改并将其合并到当前分支):
  
`git pull origin main`
    or
`git pull`



