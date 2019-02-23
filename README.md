git基本操作
来源：https://blog.csdn.net/u013497977/article/details/54291724

一 .git的安装配置（只有初次使用需要配置）
1 用户名和邮件
$ git config --global user.name "runoob"
$ git config --global user.email test@runoob.com

3 添加公钥
在右上角找到Settings->SSH keys-> Add SSH key ->拷贝在公钥（id_rsa.pub）文件中的所有的文本->完fsdf:
这样就可以使用git去连接github上的repository了。

流程
add，commit，push的区别
[（本地工作目录）——-add —–>（缓存区）—-commit——–>（本地的git库）] ——-push———>（github）

操作：
mkdir  hahaha                 本地随意创建一个文件夹
cd hahaha                      进到该目录
git init                     初始化为本地的仓库
touch readme
git add readme       每次更新都要add
#git status             查看哪些文件改变了但还未commit
#git diff                  查看文件改变的内容
git commit - m '1'     
#git status
#git log                     查看git的记录
#git checkout        撤销操作
---------------





三. 关联远程github的操作
反正必须先在github建仓库，copy库的ssh地址， 
下面1,2是两种关联方式，任选其一

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





