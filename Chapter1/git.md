# 第4节：git 命令

- `git clone ssh/https`   (如果使用ssh,需要将本地ssh需要添加到项目的ssh中)

- `git checkout -b 'name'`  (name代表想要创建的分支名称)

- `git push --set-upstream origin  'name'` (在服务器创建远程的仓库，和本地仓库名称一致)

- `git checkout 'name'` (切换到name分支)
- `git status` (查看本地分支修改了哪些内容)
- `git diff` (比较当前版本和之前的版本修改了哪些)
- `git checkout -- '路径'` (剔除不想提交的文件)
- `git add .` (添加所有文件)
- `git commit --m '注释'` (提交时候加的注释)
- `git checkout dev` 
- `git pull`
- `git checkout 'name'` (切换到name分支)
- `git merge dev` (将dev分支合并到自己的分支)
- `git checkout dev`
- `git merge 'name'`(dev合并本地的分支)
- `git push` (提交到服务器仓库)