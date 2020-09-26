## git 远程仓库

连接远程仓库

ssh-keygen -t rsa -b 4096 -C 1772492146@qq.com

git remote add oringin git @xxxxx ：

在本地添加远程仓库地址

git push -u origin master  推送本地master分支到远程origin的master分支

git clone git@?/xxx（地址）创建一个xxx目录 

clone之后马上cd xxx

git clone git@?/xxx.git  yyy 改变目录名为yyy

cd yyy

git clone git@?/xxx.git  .

使用当前的目录容纳代码和.git

先commit到本地仓库，才能push 到远程仓库







