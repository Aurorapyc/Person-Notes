# Git使用手册

-工作区 -->> 暂存区	`git add .`

-暂存区 -->> 仓库	 `git commit -m 'commit message 91'`

-查看状态			 `git status`

-看看提交记录		  `git log or git-log`

-版本回退			 `git reset --hard <commitID>`

​					-配置alias `vim ~/.bashrc`

​			             `alias git-log='git log --pretty=oneline --all --graph --abbrev-commit'`

-查看分之			 `git branch`

-创建并切换分之	   `git switch -C 分支名`

-分支合并	

​	-首先切换到目标分支上 `git switch master`

​					`git merge 需要合并的分支名`

修改分支名称-`git branch -M main`

git push [-f] [--set-upstream] [远端名称] [本地分支名] [:远端分支名] 

-f 表示强制覆盖

--set-upstream 推送到远端的同时并简历起远端分支关联关系

```python
1.删除远程仓库
	git remote rm upstream
```

```python
1.	# ![rejected]
	error: failed to push some refs to 'github.com:Auororapyc/ccy.git'
    #解决办法
    git push --set-upstream origin main
```

