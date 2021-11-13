# BASIC Interpreter - 2021


**ddl：第12周周一23:00**



## 前置工作

首先，为了score.cpp能测评你的程序：

如果你用的是wsl，请删除Basic-Demo-64bit_for_mac_to_be_rename

如果你用的是mac，请删除Basic-Demo-64bit，**并将Basic-Demo-64bit_for_mac_to_be_rename改名为Basic-Demo-64bit**

Basic-Demo-64bit是标程的可执行文件，你可以用命令行来运行它，看看BASIC解释器是如何工作的。



## 下发代码内容描述

提供了CMakeLists.txt，因此你可以直接用CLion打开下发的文件夹，直接就可以编译运行了。

你在写程序的时候只需要完成Basic文件中的内容。默认什么都不写就已经完成了一个计算器（如：输入1+1，回车，输出2），你需要自行阅读代码来判断你需要编写或增添哪些文件中的哪些部分。你也可以自行添加文件，更改类或文件的结构，不必拘泥于提供的框架，只需要在code review时向助教说明你的架构即可。

本作业会引用下发的库 StanfordCPPLib。要用到的库中的文件已经被include到各头文件中了，当然你愿意的话也可以自己使用该库的其它文件。你**不应修改**这个库中的任何内容。关于该库的使用，可以查阅官方文档[The StanfordCPPLib package](https://cs.stanford.edu/people/eroberts/StanfordCPPLib/doc/index.html)

由于StanfordCPPLib是自带内存泄漏的（用valgrind跑一遍原始下发代码就可以检测出来），**本次大作业不检测内存泄露**。

关于具体的BASIC解释器的语法要求与其它说明，请见Minimal BASIC Interpreter - 2021.pdf



## 本地测评方法

score.cpp是测评文件，会寻找你的可执行文件与Basic-Demo-64bit进行对拍（对拍，指进行相同输入看输出是否相同）。

测评文件内容默认是Test文件夹下提供的文件。这些文件和oj中测评的数据点是相同的。在这些测试点下，你的程序需要输出与标程相同的结果。

你的可执行文件路径与名字默认为`cmake-build-debug/code`,也就是CLion默认的产生可执行文件的位置。

如果路径有问题或你有独特的需求，你可以自行修改score.cpp中的路径或者测评代码来满足你的需求。



score.cpp使用方法：编译score.cpp，然后运行编译产生的文件，即可。

样例：

```
g++ -o score score.cpp
./score -f
```

使用 ./score -h 来查看帮助。



## oj提交方法

本大作业使用github进行测评。提交时，你的github仓库下需要有一个Basic文件夹，一个提供的StanfordCPPLib文件夹，与一个提供的CMakeLists.txt。



在oj的提交栏提交你的github仓库的地址，如 https://github.com/your_user_name/your_repo_name.git

（如果Compile Error，可能是因为github访问速度较慢。你只需要将提交的地址改为https://github.com.cnpmjs.org/your_user_name/your_repo_name.git形式的地址就可以进行加速了）



测评文件内容默认是Test文件夹下提供的文件。这些文件和oj中测评的数据点是相同的。在这些测试点下，你的程序需要输出与标程相同的结果。



