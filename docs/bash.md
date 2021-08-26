# GNU Bash
> notes on [github](https://github.com/jokerliang/notes)

> **本笔记参考以下文档：**
>
> https://www.gnu.org/software/bash/manual/bash.html，by GNU
>
> https://wangdoc.com/bash/index.html，by 阮一峰
>
> http://linux.vbird.org/linux_basic/0320bash.php#bash，by 鸟哥（蔡德明）
>
> https://man7.org/linux/man-pages/man1/bash.1.html

笔记练习环境

> Windows 10 V21H1
>
> Docker Desktop V3.5.2  
>
> ​	Docker Engine V20.10.7
>
> 镜像： Debian sid
>
> ​	Debian GNU/Linux 11 (bullseye) 
>
> GNU Bash V 5.1.8



## 认识Bash这个Shell



### 关于Bash

- **引用** 

> **What is Bash**
>
> Bash is the GNU Project's shell—the Bourne Again SHell. 
>
> Bash is the shell, or command language interpreter, for the GNU operating system.
>
> Bash is largely compatible with `sh` and incorporates useful features from the Korn shell `ksh` and the C shell `csh`.
>
> It currently runs on nearly every version of Unix and a few other operating systems 

- **定义**

Bash 是**壳程序** 或者叫 **命令语言解释器**，全称 Bourne Again SHell，运行在几乎所有Unix的发行版本中。

Bash高度兼容了`Bourne Shell（sh）`，并且融入了`Korn shell（ksh）`、`C Shell（csh）`的诸多实用工具；



### 关于Shell

- **引用**

>**What is a shell**
>
>At its base, a shell is simply a [^macro processor] that executes commands. 
>
>A Unix shell is both a command interpreter and a programming language.
>
>- As a command interpreter, the shell provides the user interface to the rich set of GNU utilities.  
>- The programming language features allow these utilities to be combined. Files containing commands can be created, and become commands themselves.  



>In computing, a shell is a computer program which exposes an operating system's services to a human user or other program. In general, operating system shells use either a command-line interface (CLI) or graphical user interface (GUI), depending on a computer's role and particular operation. It is named a shell because it is the outermost layer around the operating system.
>
>Command-line shells require the user to be familiar with commands and their calling syntax, and to understand concepts about the shell-specific scripting language (for example, bash).
>
>Graphical shells place a low burden on beginning computer users, and are characterized as being easy to use. Since they also come with certain disadvantages, most GUI-enabled operating systems also provide CLI shells.
>
>*via.* [wikipedia](https://en.wikipedia.org/wiki/Shell_(computing))




>我們必須要透過『 Shell 』將我們輸入的指令與 Kernel 溝通，好讓 Kernel 可以控制硬體來正確無誤的工作！ 我們可以發現應用程式其實是在最外層，就如同雞蛋的外殼一樣，因此這個咚咚也就被稱呼為**殼程式 (shell)** 囉！	
>
>只要能夠操作應用程式的介面都能夠稱為殼程式。
>
>- 狹義的殼程式指的是指令列方面的軟體，包括本章要介紹的 bash 等。 	
>- 廣義的殼程式則包括圖形介面的軟體！因為圖形介面其實也能夠操作各種應用程式來呼叫核心工作啊！ 

- **定义**

Shell，通称为[^外壳程序]，用于暴露内核（`kernel`）接口供其他程序使用；通常由操作系统启动运行后的初始化（`init`）阶段决定Shell是采用` command-line interface (CLI) `还是 `graphical user interface (GUI)`的方式向外界提供服务。

> Map of GNU/Linux Operating system internals
>
> https://makelinux.net/system/new.shtml

