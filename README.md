# Git
从本地上传文件到Github(git)

1.  打开Shell(Windows下打开Git Bash) 

2.  $ ssh-keygen -t rsa -C "youremail@example.com" （邮件地址换成你自己的邮件地址）

3.  在用户主目录里找到.ssh目录下面的 id_rsa.pub 这个文件，并将里面的内容添加到你的github账号中SSH Keys里面去

4.  登陆GitHub，创建一个新的仓库（Git）

5.  在本地创建版本库(又名仓库 英文名repository)

    $ mkdir Git
    $ cd Git
    $ pwd
    $ git init(把这个仓库变成Git可以管理的仓库)

6.  在这个Git目录下添加需要上传到远程服务器的文件，如（learn.txt）

    $ git add learn.txt //  git add learn.txt study.txt(添加多个文件) 
    $ git commit -m "first"
    
7.  根据GitHub的提示，在本地的Git仓库下运行命令：

    $ git remote add origin git@github.com:example/Git.git(本地库关联远程库)

8.  $ git push -u origin master(将内容推送到远程)
