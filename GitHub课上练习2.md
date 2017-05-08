# Github问题集（2）

## 个人主页上的“+”下拉菜单可创建的四种类别分别有？分别的意思？
1. new repository   新建一个仓库
2. import reository  导入一个仓库
3. new gist          新建一个代码片段
4. new organization   新建一个组织

## 如何能将仓库中的html文件直接解析成页面？
+ settings ->GitHub Pages->master branch ->save;

## 如何删除仓库
+ settings 里头有删除delete键

## Bash是什么操作系统的命令  
+　Linux

## Pwd是什么命令   :
+　打印当前工作目录

## Cd是什么命令   ：
+ 改变目录

## Echo是什么命令  ：
+　打印

## 配置git用户名的命令  ：
+ git config --global user.name " "


##　配置邮箱的命令
+　git config --global user.email " "

## 命令行换行方式
+ \

## 命令行终结方式
+ ctrl+c

## 使用命令行比GUI方式有何优势
+ 一次性可以提交多个编辑.....（批处理）

## 提交到本地仓库时为什么有暂存区
+ 如果修改了多个文件，是做几次的提交？由index决定，提交的次数不同，返回获得的结果也不同；

## 新建代码仓库的命令
1. mkdir demo
2. cd demo
3. git init

## git clone [url] 这个命令的作用是
+ 把远程仓库直接拉拽到本地，并且会直接建立pull和push关联；

## 添加指定文件到暂存区的命令
+ git add 文件名字

## 删除工作区文件，并且将这次删除放入暂存区的命令
+ git rm [file1][file2]


## 改名文件，并且将这个改名文件放入暂存区的命令
+ git mv[file-origin][file-renamed]

## 提交暂存区到仓库的命令
+ git commit -m "修改信息"

## 直接从工作区提交到仓库的命令
+ git commit -a -m "修改信息"

## 显示变更信息的命令
+ git status

## 查看历史信息的命令
+ git log

## Commit的意义是
+ 提交仓库，保留版本

## Pull的意义是
+ 把远程仓库的东西拉拽到本地仓库

## Push的意义是
+ 把本地仓库的东西推送到远程仓库
