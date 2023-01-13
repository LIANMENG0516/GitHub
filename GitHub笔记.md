# GitHub笔记

## 在GitHub中已经存在有库的情况下	

1. 克隆远程仓库到本地

   git clone git@github.com:LIANMENG0516/xxxxxx.git

2. 本地上传到远程仓库

   git add . （全部添加到暂存区）

   git commit -m "xxxxxxx"（全部提交, 双引号里的为注释, 比如第一次提交, 第二次提交等, 注释中英文皆可）

   git push origin master（推送到GitHub库）

## 在GitHub中没有库，但本地有文件夹的情况下

1. 在GitHub中创建库 (一般情况下库名称与本地项目文件名称也就是本地文件夹名称相同)

2. 在本地文件夹中点击鼠标右键-点击 Git Brash Here 调出Git终端输入以下命令

   git init

   git remote add origin git@github.com:michaelliao/learngit.git   (关联本地Git库与GitHub上的库)

   git add .

   git commit -m "xxxxxxx"

   git push origin master


## GitHub库分支与合并

### 在GitHub中创建分支

1. 在GitHub中操作并创建分支	(假设分支名为xxx)

2. 克隆GitHub中的库到本地，则克隆后的本地库就包含两个分支一个主分支master，另外一个分支为xxx

3. 在克隆到本地的库中右键调出Git终端使用如下命令切换至xxx分支，并提交

    git checkout xxx

    git add .

    git commit -m "xxxxxxx"

    git push origin xxx

### 在Git中创建分支

1. 双击打开本地Git库，右键调出Git终端使用如下命令创建分支（假设分支名为xxx）

    git branch xxx

2. 切换到xxx分支并，使用如下命令提交

    git checkout xxx

    git add .

    git commit -m "xxxxxxx"

    git push origin xxx

### 合并到主分支

1. 切换到主分支

    git checkout master

2. 合并分支到当前分支（假设需要合并的分支为xxx）

    git merge xxx

## 小结

1. 查看分支

    git branch

2. 删除分支（假设需要删除的分支为xxx）

    git branch -d xxx

# TEST
