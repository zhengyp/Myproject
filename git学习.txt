git 使用方法

1 注册github账号

2 下载git客户端 gitbash

3 mkdir /d/opt/repository创建本地仓库   git init创建git配置文件

4 git与github之间的传输是通过SSH加密的，所以第一步先在本地生成一.ssh   cd ~/.ssh  先查看本地是否有.ssh文件，有的话删掉

5 输入命令，生成.ssh，写你自己的邮箱   ssh-keygen -t rsa -C "your email@.com"

6 为了避免与github创建连接时出错，可以新建一个config文件，将以下代码复制进去   Host github.com
    User git
    Hostname ssh.github.com
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
    Port 443


7 将id_rsa.pug的内容复制到指定位置  头像  setting  ssh and gpg keys 

8 测试连接是否成功，下图表示访问成功	ssh -t git@github.com

9 上传项目 git add <文件名>   git commit -m "first commit" 

   git remote add origin git@github.com:zhengyp/Myproject.git

   如果出错  git remote rm origin 后继续上一步

10 git push -u origin master

11 更新文件 git add readme.txt  git commit -m "优化二进宫"   git push -u origin master 

12 开始学习分支相关部分