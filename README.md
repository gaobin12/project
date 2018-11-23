# project
练习

create a project
# react

#git 命令

cd 切换目录

mkdir 创建目录

rm 删除

mv 移动

pwd 查看根目录

vim 启动编辑器

esc 退出 ：wq保存

git config --global --list 查看配置信息

git config --global user.name "" 配置用户名

git config --global user.email "" 配置邮箱
# git上传步骤
git init

git add *

git commit -m ""

git pull --rebase origin master 这一句可以代替以下两句

git fetch

git merge

#git 从安装到与远程项目交互

下载 git 

配置git用户信息 git config --global user.name "xxx"
git config --global user.email "xxx"

获取密钥 ssh-keygen -t rsa -C 邮箱 一直回车

在github的settings中找到ssh配置 创建连接

测试连通性 git -T git@github.com  连接成功会在 /.ssh目录下 多一个新文件known_hosts

本地项目与远程项目关联 git remote add origin https://gaobin12/demo.git

#第一次上传（本地到远程）

git init 初始化

git add . 添加到暂存区

git commit -m "添加到本地分支 默认主分支 这里写说明"

git push -u origin master 推送到主分支

#第一次远程到本地

git clone https://gaobin12/demo.git(在github项目中复制即可)

再次提交

git add .

git commit -m "说明"

git push origin master 推送

拉取 git pull 



修改文件

git add *

git commit -m ""

git push -u origin master

#取消本地目录下关联的远程库

git remote remove origin
