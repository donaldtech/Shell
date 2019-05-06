## JDK
```
JDK>JRE>JVM实例
Oracle JDK 8 / OpenJDK 8 / IBM J9 JDK 8
下载 
https://www.oracle.com/technetwork/java/javase/downloads/index.html


安装 
windows
默认
环境变量 Control Panel\System and Security\System\Advanced System Setting\Enviroment Variables\
JAVA_HOME=C:\Program Files\Java\jdk-12
Path=C:\Program Files\Java\jdk-12\bin
验证 cmd: javac -version


目录结构
bin-可执行命令
  javac-Java编译器
  java-运行编译后的JVM应用程序，即使这种程序不是使用Java写的
  桌面GUI监视工具
     jvisualvm  from http://visualvm.github.io/
     jmc
include-供C语言编译器使用的头文件
lib-库
```

## 用包组织类
```
同一包中的类构成了一个命名空间
包         包中的类
basket     Basket,BasketLine-describe sth
product    Product
com.example.jvm_university.webprogramming

package com.example.jvm_university.webprogramming;
class Application {
}
全限定类名com.example.jvm_university.webprogramming.Application
````

## 类库=API
```
类库中的所有类放在包（java...  javax.... org.xml com.oracle...）中
包               类库中的类
java.lang        String, StringBuilder, Object
java.io/net/nio  操作系统，文件，网络IO的类
java/javax.sql   访问JDBC的类

java.lang包
java,lang.Object类

java.lang.String类
java.lang.Number

java.lang.Exception
java.lang.Error

java.util.ArrayList
java.util.HashMap
```


## 第一个java程序
vim HelloWorld.java(文件名需与类名一致)
```
public class HelloWorld {  
    public static void main(String[] args) { //主方法入口：所有的 Java 程序由 public static void main(String []args) 方法开始执行
        System.out.println("Hello World");
    }
}

//类名大大大
//方法名小大大
关键字

访问控制	private	私有的 / protected	受保护的 / public	公共的

类、方法和变量修饰符	abstract	声明抽象 / class	类 / extends	扩充,继承 / final	最终值,不可改变的  implements	实现（接口） / interface	接口 / native	本地，原生方法（非 Java 实现）/ new	新,创建 / static	静态

包相关	import	引入 / package	包

变量引用	super	父类,超类 / this	本类 / void	无返回值


$ javac HelloWorld.java   将 java 源文件编译为 class 字节码文件 (HelloWorld.class)
$ java HelloWorld  java文件中的类名
```

## 基础语法
### 对象和类
```
类
public class Dog{
  String breed;
  int age;
  String color;
  void barking(){
  }
 
  void hungry(){
  }
 
  void sleeping(){
  }
}
```
### 基本数据类型
### 变量类型
### 修饰符
### 运算符
### 循环结构
### 条件语句
### switch case
### Number Math类
### Character类
### String类
### StringBuffer
### 数组
### 日期时间
### 正则表达式
### 方法
### Stream File IO
### Scanner类
### 异常处理
## 面向对象

## 高级编程
