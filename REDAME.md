git基本操作
来源：https://blog.csdn.net/u013497977/article/details/54291724

初次使用需配置用户名和邮箱
1 用户名和邮件
$ git config --global user.name "runoob"
$ git config --global user.email test@runoob.com


add，        commit，  push 的区别 

[（本地工作目录）——-add —–>（缓存区）—-commit——–>（本地的git库）] ——-push———>（github）  

mkdir  hahaha               本地随意创建一个文件夹
cd hahaha                      进到该目录
git init                     初始化为本地的仓库
touch readme
git add readme       每次更新都要add
git status             查看哪些文件改变了但还未commit
git diff              
git commit - m '1'     
git status
git log                     查看git的记录
git checkout        撤销操作



1
github创建仓库hahaha之后,把github上的git下载到本地
git clone  git@github.com:username/hahaha.git

2
github创建hahaha，把本地的库hahaha与github上的git关联
git remote add origin git@github.com:username/hahaha.git

3
把本地的东西都推上去
 git push -u origin master/
把上面的都下下来
 git pull




