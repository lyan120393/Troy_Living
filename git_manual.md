Git 使用方法参考
说明： git 不是 github。git是一套代码管理的机制，如同svn。


## Git 库基本操作
### 创建项目

	$ git init 

### 添加文件 （编辑）

	$ git add .

### 添加远程 git地址

	$ git remote add <your-github-repo-ssh-url>

### 删除文件

	$ git rm <filename>

### 提交项目

	$ git commit -am "commit sentences"

### 推送项目

	$ git push origin <branch_name>

### 拉取项目（更新）

	$ git pull origin <branch>


## 分支操作
### 创建分支

	$ git branch <branch_name>

### 切换分支

	$ git checkout <branch_name>

### 合并分支

	$ git merge <target_branch>

### *变基（rebase）

	$ git rebase <target_branch>

## 更多帮助

	$ git --help

常用 git库 结构

	master
	|
	 - fix
	|
	 - main
	 	|
	 	 - Backend - Module A - Function A
	 	|		  |			 |
	 	|		  |			 |
	 	|		  |			  - Function B
	 	|		  |
	 	|		   - Module B - Function C
	 	|		  			 |
	 	|		  			 |
	 	|		  			  - Function D
	 	|
	 	 - Front_End - ...

## 正规操作流程
### 警告：不要编辑 master 分支
### 第一次获取项目
$ git init 
$ git remote add <your-github-repo-ssh-url>

### 编辑上传代码
$ git pull origin <branch>
$ git add .
$ git commit -am "notes"
$ git push origin <branch>

