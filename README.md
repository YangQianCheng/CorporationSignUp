社团报名系统
============
###0.准备工作
* 先注册一个Github账号，然后来项目这里`fork`一下。
* 如果使用Windows平台下的GUI程序，可以到群里下载我刚分享的离线安装包；建议使用一起安装上的`Git Shell`（欢迎尝试使用[`Cygwin`][2]或者[`msysGit`][3]），关于fork的操作可以看[这里][1]。
* 可以先自己新建项目练习一下Github的相关操作（不论是GUI程序操作还是命令行操作），关键是掌握团队协作发布代码的流程。

###1.团队协作流程
#### 1.1克隆版本库
* 下载并安装Github for Windows的GUI程序。
* 点击项目主页右下方`Clone in Desktop`，或者在PowerShell中切换到合适的目录，并运行命令
`git clone https://github.com/PengEdy/CorporationSignUp.git`

####1.2配置远程连接
    cd CorporationSignUp
    git remote add upstream https://github.com/PengEdy/CorporationSignUp.git
    git fetch upstream

####1.3从远程更新本地的版本库

    git pull
或

    git fetch upstream
    git merge upstream/master

####1.4添加文件到本地版本库
以`index.html`为例，也可以使用通配符`*`。

    git add index.html
    git commit -m "your name: balabala..."
注意commit格式：`姓名：提交说明`

####1.5提交本地版本库到远程库
    git push origin master

###2.注意事项
* 发布的repo中不要出现中文路径名称（包括文件夹名和文件名）。
* 在项目过程中，如出现任何关于Github的问题，自己不确定的情况下不要擅自解决，可以来找我。

[1]: https://help.github.com/articles/fork-a-repo
[2]: http://www.cygwin.cn/
[3]: http://msysgit.github.io/
