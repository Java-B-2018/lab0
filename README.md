# Lab0

这是Programming课程的第一次上机实验，本次Lab旨在帮助大家配置好相应地环境，为日后的编程做准备

## 目录
- [教学团队](#教学团队)  
- [Lab课堂要求与建议](#lab课堂要求与建议)
- [使用学院的ftp](#使用学院的ftp)
- [使用elearning](#使用elearning)
- [安装Java JDK](#安装java-jdk)
- [软件的选择的建议](#软件推荐)


## 教学团队
### 教师：陈荣华
联系方式：[chenrh@fudan.edu.cn](http://chenrh@fudan.edu.cn)
### 助教：
- 何宇雯 [15302010042@fudan.edu.cn](http://15302010042@fudan.edu.cn) 13321961355
- 姚鹏 [16302010057@fudan.edu.cn](http://16302010057@fudan.edu.cn) 17621191357
- 阮家炜 [16302010028@fudan.edu.cn](http://16302010027@fudan.edu.cn) 18950563903

## 任务

- 熟悉计算机操作及命令

- 使用ftp上传下载作业

- 配置环境（含java）

- 运行第一个程序

## Lab课堂要求与建议  
1. 遇到问题请先自我思考，再考虑使用Google，最后再询问周围的同学和助教。  
2. 在完成Lab后和周围的同学进行语言上得交流和代码上的交流(Code Review)，积极地讨论。  
3. 按时、按说明递交作业，如有情况请及时向TA通过邮件说明。  
4. 如果你不是大牛，请亲自来Lab课并当堂完成。当你抄了一个lab，会根本停不下来，起码学长学姐的历史上经常是这样的。程序设计有五学分，而且是编程生涯的第一堂课，抄袭的下场可能有点惨：）


## 使用学院的ftp


FTP 站点类似于云盘，在FTP上可以下载软件学院的的课程资料，我们主要使用 FTP 提交每次 lab 作业 和期中期末两次 Project

进入FTP之前**必须连上学校内网**

源地址：```ftp://10.132.141.33```

![figure](https://cloud.githubusercontent.com/assets/6169077/18310556/a7004386-7531-11e6-99c0-4918f8976bfe.png)

1. 使用ftp客户端或者Windows资源管理器，在学校内网下访问，用户名与密码都是学号，登入之后请改密码。

2. 还有一个无门槛的账户（用户名 ```ss``` 密码 ```ss```），提供紧急使用。

3. Mac端推荐使用fileZilla作为客户端，地址在学院文件夹里。

4. 然后进入 ```/classes/18/181 程序设计A（陈荣华）```

![child](https://raw.githubusercontent.com/Java-B-2018/lab0/master/images/child.PNG)


>注意，你只对 WORK_UPLOAD文件夹有上传的权限，没有下载、删除、重命名的权限。  
请重命名文件后再上传，ftp服务器上错误的文件名是无法修改的，但是可以 覆盖重名的文件。

## 使用elearning

浏览器打开  
http://elearning.fudan.edu.cn/portal  
右上角使用 URP 账号登陆。

## 安装java JDK

请在 FTP 的 Materials 文件夹或者 Java 官网下载符合电脑操作系统的JDK版本安装包并安装： [JDK 1.8](https://www.oracle.com/technetwork/cn/java/javase/downloads/jdk8-downloads-2133151-zhs.html) 。


### 配置环境变量（Windows）

1. 在桌面上右键`计算机`(或者`此电脑`，`我的电脑`，不同系统显示名称可能不同)，点击`属性`:
2. 点击`高级系统设置`
3. 点击`环境变量`
4. 在`系统变量`中，选中名为`Path`的条目，点击编辑。

   ![](https://cloud.githubusercontent.com/assets/6532225/18434149/11c793c8-791e-11e6-9f41-63ea328452e6.png)

   如果使用的是Windows 10，点击新建，输入`C:\Program Files\Java\jdk1.8.0_101\bin`，确定。

   ![](https://cloud.githubusercontent.com/assets/6532225/18434153/14159efe-791e-11e6-87dc-8570af650adf.png)

   命令行会从上图中所有的路径中搜索你输入的命令。在我们把目录添加进去后，不管在哪个文件夹下，命令行都能找到`java`和`javac`。

5. 接下去我们配置`CLASSPATH`。

   在`系统变量`中，点击`添加`，`变量名`填`CLASSPATH`，`变量值`填`.`，确定。

   ![](https://cloud.githubusercontent.com/assets/6532225/18438460/0bc3c558-7934-11e6-8cce-8dd27d1135a2.png)

Windows 7 和 Windows 8 的配置在界面上有一些小区别，可以参考
[http://jingyan.baidu.com/article/925f8cb836b26ac0dde0569e.html](http://jingyan.baidu.com/article/925f8cb836b26ac0dde0569e.html)

在这个链接中，还添加了一些其他的路径到Path和CLASSPATH，这个是过时的做法，高版本的Java不需要这样设置。



### 配置环境变量（macOS）

打开终端，输入以下命令：

```
echo -e 'export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_181.jdk/Contents/Home\nexport CLASSPATH=.\n
export PATH=${PATH}:${JAVA_HOME}\n' >> ~/.bash_profile
```





### 第一个Java程序： Hello world！
**对于检查环境配置，能打印出一句话说明路径、环境配置基本成功。**

用记事本或文本编辑器在电脑上新建文件 ```Main.java``` ，输入  
```
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

+ 在当前目录打开powershell命令行
![powershell](https://raw.githubusercontent.com/Java-B-2018/lab0/master/images/powershell.png)

+ 输入编译指令并运行程序
![HelloWorld](https://raw.githubusercontent.com/Java-B-2018/lab0/master/images/HelloWorld.png)

## 软件推荐

集成环境（IDE，**极力推荐**）:

+ [IntelliJ IDEA](http://www.jetbrains.com/idea/)



文本编辑器：

+ [Visual Studio Code](https://code.visualstudio.com/) (**极力推荐**)
+ [Atom](https://atom.io/) (**推荐**)
+ [NotePad++](https://notepad-plus-plus.org/)
+ [Sublime Text](https://www.sublimetext.com/)

浏览器：
 + [Google Chrome](https://www.google.cn/chrome/)
 + [Mozilla FireFox](http://www.firefox.com.cn/)

搜索引擎：

+ [Google](https://www.google.com.hk/)

搜集材料（当然只是借鉴）：
 + [CSDN](https://blog.csdn.net/)
 + [Github](https://github.com/)
 + [PUDN](http://www.pudn.com/)
