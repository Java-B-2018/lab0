#Lab0

这是Programming课程的第一次上机实验，本次Lab旨在帮助大家配置好相应地环境，为日后的编程做准备。

[教学团队](#教学团队)  
[Lab课堂要求与建议](#要求)
[关于操作系统](#操作系统)
[使用学院的ftp](#ftp)
[使用elearning](#elearning)
[安装Java JDK](#安装java&nbspJDK)
[配置环境变量](#配置环境变量)
[Hello World!](#Helloworld)
[软件的选择的建议](#软件推荐)
[提交](#提交)

##教学团队
###教师：陈荣华
联系方式：[chenrh@fudan.edu.cn](http://chenrh@fudan.edu.cn)
###助教：
何宇雯 [15302010042@fudan.edu.cn](http://15302010042@fudan.edu.cn) 13321961355
姚鹏 [16302010057@fudan.edu.cn](http://16302010057@fudan.edu.cn) 17621191357
阮家炜 [16302010028@fudan.edu.cn](http://16302010027@fudan.edu.cn) 18950563903

##任务

- 熟悉计算机操作及命令

- 使用ftp上传下载作业

- 配置环境（含java）

- 运行第一个程序

##Lab课堂要求与建议  
1. 遇到问题请先自我思考，再考虑使用Google，最后再询问周围的同学和助教。  
2. 在完成Lab后和周围的同学进行语言上得交流和代码上的交流(Code Review)，积极地讨论。  
3. 按时、按说明递交作业，如有情况请及时向TA通过邮件说明。  
4. 如果你不是大牛，请亲自来Lab课并当堂完成。当你抄了一个lab，会根本停不下来，起码学长学姐的历史上经常是这样的。程序设计有五学分，而且是编程生涯的第一堂课，抄袭的下场可能有点惨：）

##关于操作系统

本文档主要针对Windows系统，对于Linux和OS X也会提供相应支持。

##使用学院的ftp

源地址：<ftp://10.132.141.33>

1. 然后进入classes，年级，进入所选课程。

2. 使用ftp客户端或者Windows资源管理器，在学校内网下访问，用户名与密码都是学号，登入之后请改密码。

3. 还有一个无门槛的账户，提供紧急使用。

4. 用户名 ss 密码 ss

5. Mac端推荐使用fileZilla作为客户端，地址在学院文件夹里。

6. 上传你自己的lab文件，在各自的年级的课程的work_upload中

>注意，你只对 WORK_UPLOAD文件夹有上传的权限，没有下载、删除、重命名的权限。  
请重命名文件后再上传，ftp服务器上错误的文件名是无法修改的，但是可以 覆盖重名的文件。

##使用elearning

浏览器打开  
http://elearning.fudan.edu.cn/portal  
右上角使用 URP 账号登陆。

##安装java JDK

###配置环境变量

###Hello world！
对于检查环境配置，能打印出一句话说明路径、环境配置基本成功。  
用文本编辑器在Lab目录（自己建的）下新建文件 Lab0.java ，输入  
```
public class Lab0 {  
    public static void main(String[] argv) {  
        System.out.println("Hello World !");  
    }  
} 
```
> 请注意，文件名要与public class的类名一致！

然后在命令行中切换目录到lab目录下。切换目录使用 cd 命令， .表示当前目录，..表示上一  
层目录，例如：  
C:\\User\\htc\>d:  
D:\\\>cd LAB  
D:\\LAB\>cd LAB0  
D:\\LAB\\LAB0\>cd ..  
D:\\LAB\>cd .  
D:\\LAB\>cd LAB0  
D:\\LAB\\LAB0\>  
请注意，文件夹的命名是大小写敏感(Case
Sensitive)的，LAB和lab对应的是两个不同的文件！  
（夹）。在命令行中用TAB键补全往往可以省去很多功夫！  
现在，让我们编译、运行第一个 Java 程序！  
注意：javac是进行程序编译的工具，java是用于程序运行的工具。  
D:\\LAB\\LAB0\>javac Lab0.java  
D:\\LAB\\LAB0\>java Lab0  
Hello World !

软件推荐

文字编辑器：NotePad++,Atom,Sublime Text等

集成环境（IDE）:Java推荐用IntelliJ IDEA,Python推荐用PyCharm,C++推荐用Visual
Studio(Windows)或者Xcode（OS X）

浏览器：Google,FireFox

搜索引擎：Google

搜集材料：csdn,pudn,github(当然只是借鉴)

提交  
将你的 LAB0
目录（至少包（至少包含Lab0.java文件）打包成zip或者rar格式的文件，重命名为学号,提交到指定的目录下。
