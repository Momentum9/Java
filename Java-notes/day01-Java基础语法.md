# day01 - Java基础语法

## 1. 常用CMD命令

常见的CMD命令如下：

| 操作               | 说明                              |
| ------------------ | --------------------------------- |
| 盘符名称:          | 盘符切换。E:回车，表示切换到E盘。 |
| dir                | 查看当前路径下的内容。            |
| cd 目录            | 进入单级目录。cd itheima          |
| cd ..              | 回退到上一级目录。                |
| cd 目录1\目录2\... | 进入多级目录。cd itheima\JavaSE   |
| cd \               | 回退到盘符目录。                  |
| cls                | 清屏。                            |
| exit               | 退出命令提示符窗口。              |



## 2. Java概述

#### 1.2.3 JDK的安装目录介绍

| 目录名称 | 说明                                                         |
| -------- | ------------------------------------------------------------ |
| bin      | 该路径下存放了JDK的各种工具命令。javac和java就放在这个目录。 |
| conf     | 该路径下存放了JDK的相关配置文件。                            |
| include  | 该路径下存放了一些平台特定的头文件。                         |
| jmods    | 该路径下存放了JDK的各种模块。                                |
| legal    | 该路径下存放了JDK各模块的授权文档。                          |
| lib      | 该路径下存放了JDK工具的一些补充JAR包。                       |



#### 2.3.1 Java程序开发运行流程

开发Java程序，需要三个步骤：编写程序，**编译**程序，**运行**程序。

#### 2.3.2 HelloWorld案例的编写

1. 新建文本文档文件，修改名称为HelloWorld.java。

2. 用记事本打开HelloWorld.java文件，输写程序内容。

```java
public class HelloWorld {
	public static void main(String[] args) {
		System.out.println("HelloWorld");
	}
}
```

3. 保存

4. **编译**文件。编译后会产生一个class文件。

   java文件：程序员自己编写的代码。

   **class文件：交给计算机执行的文件。**

5. **运行**代码

   **注意**：运行的是编译之后的class文件。

用到两个命令：

​	==javac== + 文件名 + 后缀名 （**编译**java文件）

​	==java== + 文件名（**运行**编译之后的class文件）



![image-20220706115513755](https://cdn.jsdelivr.net/gh/Momentum9/pictures/img/202207081017091.png)

![image-20220706115439899](https://cdn.jsdelivr.net/gh/Momentum9/pictures/img/202207081017093.png)

### 1.7 Java语言的发展

三个版本：

* Java5.0：这是Java的第一个大版本更新。
* Java8.0：这个是目前绝大数公司正在使用的版本。因为这个版本最为稳定。
* Java15.0：这个是我们课程中学习的版本。



### 1.8 Java的三大平台

​	JavaSE、JavaME、JavaEE

#### 1.8.1 JavaSE

​	是其他两个版本的基础。

#### 1.8.2 JavaME

​	Java语言的小型版，用于嵌入式消费类电子设备或者小型移动设备的开发。

​	其中最为主要的还是小型移动设备的开发（手机）。渐渐的没落了，已经被安卓和IOS给替代了。

​	但是，安卓也是可以用Java来开发的。

#### 1.8.3 JavaEE

​	用于Web方向的网站开发。（主要从事后台服务器的开发）

​	在服务器领域，Java是当之无愧的龙头老大。

### 1.9 Java的主要特性

- 面向对象
- 安全性
- 多线程
- 简单易用
- 开源
- 跨平台

#### 1.9.1 Java语言跨平台的原理

- 操作系统本身其实是不认识Java语言的。
- 但是针对于不同的操作系统，Java提供了不同的虚拟机。

虚拟机会把Java语言翻译成操作系统能看得懂的语言。

![image-20210923091350952](https://cdn.jsdelivr.net/gh/Momentum9/pictures/img/202207081017094.png)

### 1.10 JRE和JDK

![image-20210923091544110](https://cdn.jsdelivr.net/gh/Momentum9/pictures/img/202207081017095.png)

JVM（Java Virtual Machine），Java虚拟机

JRE（Java Runtime Environment），Java运行环境，包含了JVM和Java的核心类库（Java API）

JDK（Java Development Kit）称为Java开发工具，包含了JRE和开发工具

总结：我们只需安装JDK即可，它包含了java的运行环境和虚拟机。
