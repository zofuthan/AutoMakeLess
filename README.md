AutoMakeLess
========
一个简单的Less监视编译软件,支持windows,mac,linux,通过网页进行管理.

#注意
  使用前确保已经正确安装了node和less,并能够在命令行中执行lessc    
  [安装方法](http://iyf.cc/archives/413)

#功能
  1. 文件变更监视,当文件创建,修改,删除,改名都会在第一时间进行处理.    
    1.1 文件创建时会自动进行编译,如果这个文件是从其他地方拷贝过来,也会立即编译    
	1.2 文件修改时将在文件所在位置立即重新编译`*.css`文件.    
	1.3 文件删除时会自动删除同名的`*.css`文件.    
	1.4 文件改名时会将原名称同名的css文件删除,并编译新名称的css文件.
  2. 编译错误提示,如果编译出错可单击页面中的失败按钮查看错误信息,并会在less文件修改后重新编译.
  3. 监视目录以及子目录,并且被监视目录下新创建的目录会自动加入到监视列表,使用时只需要将项目所在路径加入,整个项目中所有的less文件都会被监视.
  4. 跨平台使用,提示信息通过网页来展示.
  5. 使用`-addr=端口号`即可以自定义端口运行

#已编译版本
如果不想自己编译程序请在这里下载已经编译的程序.
[已编译版本](http://iyf.cc/archives/429 "AutoMakeLess,一个简单的跨平台自动less编译工具")

#使用注意
+ 启动程序后必须访问一次本页面才会启动监视.然后关闭浏览器也会继续执行.
+ 当修改文件或增加文件,页面提示信息需要手动刷新才可以看到变化
+ 修改后缀后需要重新启动程序.
+ 点击退出程序后后台进程自动关闭
+ 修改编译参数后需要手动点击`重新编译列表项`
+ 出现编译错误的项点击失败即可看到错误信息
+ 删除`*.less`文件并且该文件被监视,那么会同时自动删除`*.css`文件
+ 改名`*.less`文件会自动删除与该文件同名的css文件,并会自动建立改名后的css文件
+ 程序会自动处理加入监视的目录下级新建立的目录,无需增加路径,但是这部分路径并不会显示在列表.

#作者
于风:[http://iyf.cc/](http://iyf.cc/ "我的博客")
