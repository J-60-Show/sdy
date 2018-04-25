## IntelliJ IDEA设置TortoiseSVN插件(Cannot run program "svn")


IntelliJ IDEA 2016.3.4版本本身己集成各种版本管理工具，不过真正要用时还得先配置好
![Enjoy](https://raw.githubusercontent.com/J-60-Show/sdy/master/Res/20170227170657408.png)
打开设置页面

![Enjoy](https://raw.githubusercontent.com/J-60-Show/sdy/master/Res/20170227170800132.png)

需要设置一个svn.exe的路径，而大多数人安装后的TortoiseSVN\bin都没有svn.exe这个文件
没设置好就用SVN功能的话会报错
`Cannot run program "svn"`
这要求你在安装TortoiseSVN时把它的命令行客户端功能也安装，才能通过命令执行版本管理

![Enjoy](https://raw.githubusercontent.com/J-60-Show/sdy/master/Res/20170227170903634.png)
运行安装程序，然后到了这一步时把第二个选项勾上，就行了。
安装后重新回IDEA的设置，把bin/svn.exe路径设置好就能用了
